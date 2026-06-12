# Modèle actuariel d'amortissement de la prime d'émission

## Cadre

Ce document décrit le modèle d'amortissement actuariel de la prime d'émission
d'une obligation, sous la forme d'une « boîte noire » à état minimal.

Conventions retenues :

- raisonnement en **monnaie courante**, sans retraitement d'inflation ;
- décompte des jours en **ACT/365**, sans recours aux conventions de marché
  (ACT/ACT, 30/360, etc.) : un coupon tombe à sa date, point ;
- pas de distinction *clean / dirty* : la boîte ne connaît que des entrées et
  des sorties d'argent à des dates données ;
- l'instrument peut être libellé en devise étrangère ; les flux sont convertis
  au taux du jour, le coût de revient à un taux historique moyen pondéré.
- le coupon couru réglé à l'achat est inclus au coût moyen pondéré
  d'acquisition

La contrainte de cohérence est qu'**au dénouement, la somme des intérêts
déclarés soit égale à l'enrichissement économique** : aucune perte sèche ne
doit être générée, à un centime d'arrondi près.

## Variables d'état

L'état de la boîte à une date donnée est entièrement décrit par cinq variables :

| Symbole | Désignation | Unité |
| ------- | ----------- | ----- |
| `C`   | coût ajusté | € (au taux historique `x_h`) |
| `x_h` | taux de change historique moyen pondéré | € par unité de devise locale |
| `U`   | intérêts internes non réalisés | € (au taux en vigueur lors de leur génération) |
| `t0`  | date de référence (dernier événement) | date |
| `r`   | taux actuariel (TRI) annuel | sans dimension, exprimé en devise locale |

On a par construction `C = C_local · x_h`, où `C_local` est le coût ajusté
exprimé en devise de l'instrument. Les accrétions d'intérêts se calculent
naturellement en devise locale puis se convertissent ; comme `C` est en € au
taux historique, l'accrétion `C · [(1+r)^τ − 1]` donne directement la part
d'intérêts valorisée à ce même taux historique.

Ces cinq variables forment un **état de Markov** : connaissant le calendrier
des flux à venir, toute la fiscalité future en découle, sans recours à
l'historique.

## Événements

On note `τ = (t − t0) / 365` la fraction d'année écoulée depuis le dernier
événement, `x_d` le taux de change du jour, et `δ = C · [(1+r)^τ − 1]` la part
d'intérêts accrue depuis `t0` (en €, au taux historique).

### Coupon (sortie d'argent)

À la réception d'un coupon de montant `K` (devise locale) à la date `t` :

```
δ  = C · [(1+r)^τ − 1]          # intérêts accrus, € au taux historique
a  = K · x_h − δ                # part d'amortissement (retour de capital)
C  ← C − a                      # le coût ajusté décroît vers le pair
I  = K · x_d − a + U            # intérêt imposable de la période
U  ← 0                          # purge des intérêts internes
t0 ← t
```

L'intérêt imposable se réécrit `I = δ + U + K · (x_d − x_h)` : la part
d'intérêts actuariels, augmentée des intérêts internes éventuels, augmentée du
gain de change sur le coupon. Tout surplus de change (et, le cas échéant,
d'indexation) est ainsi **mécaniquement reversé sur la ligne des intérêts**,
jamais sur le capital. En l'absence de change (`x_d = x_h = 1`), on retrouve
`I = δ + U`.

### Achat supplémentaire (entrée d'argent)

À un apport `A` (devise locale) à la date `t`, en cours de période :

```
δ   = C · [(1+r)^τ − 1]                 # intérêts internes accrus
U   ← U + δ                             # parqués au taux historique courant
C   ← C + δ + A · x_d                   # mise à niveau puis ajout de l'apport
x_h ← C / ( (C − A·x_d)/x_h + A )       # nouveau taux historique pondéré
r   ← TRI(C/x_h, flux locaux restants)  # recalcul actuariel
t0  ← t
```

L'apport dilue le taux historique : `U` est figé au **taux historique
antérieur** avant dilution (c'est pourquoi `U` est stocké en €). Le nouveau
taux actuariel `r` se résout sur le coût ajusté en devise locale `C/x_h` et le
calendrier des flux restants.

### Cession (sortie partielle de capital)

Pour la cession d'une fraction `f` du nominal détenu, à la date `t`, produit
`P` (devise locale) :

```
G  = P · x_d − C · f      # résultat de cession (€)
C  ← C · (1 − f)
U  ← U · (1 − f)
```

`x_h`, `r` et `t0` sont inchangés. La cession est un **événement de capital** :
`G` relève des plus ou moins-values mobilières, non des produits de placement à
revenu fixe. Les intérêts internes ne sont **pas cristallisés** : la fraction
cédée de `U` n'a plus de coupon à venir pour la solder, et se trouve absorbée
dans `G` puisque le coût ajusté `C·f` n'inclut pas ces intérêts non encore
portés. Sur la durée de vie, le total reste conservé.

### Remboursement

Le remboursement est un coupon de montant `K = dernier coupon + nominal`. Le
mécanisme du coupon conduit `C` au pair (`C → 0` à un centime près) ; la part
d'intérêts résiduelle, augmentée de `U`, constitue le dernier intérêt
imposable.

## Décomposition par lot

Chaque acquisition peut être traitée comme un **lot indépendant**. Un lot ne
reçoit jamais d'apport ultérieur (par définition, tout apport est une nouvelle
acquisition, donc un nouveau lot) : à l'intérieur d'un lot, `U` est donc
toujours nul aux dates de coupon et `x_h` reste fixe. Le lot se réduit alors à
un simple tableau d'amortissement déterministe, calculable une fois pour toutes
à l'acquisition, du type d'un crédit amortissable classique.

Le modèle agrégé est strictement équivalent à la somme des lots. Tout y est
linéaire — coûts ajustés additifs, intérêts internes additifs, taux historique
en moyenne pondérée, cession au prorata du nominal — **à la seule exception du
recalcul du taux actuariel** lors d'une fusion de lots, qui requiert une
résolution non linéaire.

C'est précisément cette unique non-linéarité qui justifie de **conserver les
lots séparés** : la décomposition par lot évite toute fusion, produit des
tableaux d'amortissement auditables ligne à ligne, et donne des déclarations
identiques au modèle agrégé. La règle française du coût unitaire moyen pondéré
est satisfaite par la répartition proportionnelle des cessions.

## L'unique non-linéarité

Tout le modèle repose sur une seule opération non linéaire : la détermination
du taux actuariel `r` solution de

```
Σ_i  F_i / (1 + r)^(j_i / 365)  =  C_local
```

où les `F_i` sont les flux restants et `j_i` le nombre de jours qui les sépare
de la date de valeur. Cette résolution s'effectue une fois par lot à
l'acquisition (méthode de Newton ou de Brent). Tout le reste — tableau
d'amortissement, ventilation intérêts / capital, conversion en €, cession
partielle, agrégation des lots — est de l'arithmétique linéaire.

## Arrondi et centime résiduel

Les accrétions se calculent à pleine précision en devise locale ; la conversion
en euros et l'arrondi n'interviennent qu'au moment de la déclaration. La dérive
d'arrondi cumulée sur la durée de vie laisse au remboursement un résidu de
l'ordre du centime, qui se déclare comme dernière fraction d'intérêt. Ce résidu
non nul est une marque de calcul actuariel effectif : un zéro parfait
trahirait au contraire une approximation arrondie.
