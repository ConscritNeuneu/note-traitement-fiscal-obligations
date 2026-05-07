# Fiscalité des obligations pour les particuliers

## Cadre de la discussion

Dans toute la suite de la discussion, nous ne nous intéressons qu'aux
obligations « typiques », *non indexées*, telles que l'État français en
émet, avec remboursement « au pair ».

La discussion ne concernera que la fiscalité pour les personnes physiques.

La présente note raisonne en *monnaie courante*. Elle ne traîte pas de la
question, distincte, de l'imposition de gains nominaux liés à l'inflation.
Ainsi les termes « revenu », « enrichissement », « assiette » doivent être
compris sans correction monétaire ni retraitement lié à l'inflation.

La question étudiée n'est pas celle de l'imposition de l'inflation, mais
celle de la qualification de flux financiers obligataires entre revenu et
restitution de capital.

## Rappel sur les obligations

### Généralités

Les obligations sont des instruments négociables sur les marchés financiers
et le moyen principal pour les États, entités publiques et les grandes
entreprises de lever de la dette.

Une obligation est caractérisée par un nominal (grossièrement, la valeur d'une
unité de dette), une maturité (la durée de remboursement) et le taux de
coupon. L'émetteur s'engage à verser pendant la durée de remboursement un
coupon à intervalles périodiques (la plupart du temps annuels). À la fin de la
période de remboursement, un dernier coupon est versé ainsi que le nominal en
guise de dénouement.

En règle générale, à l'émission, les acheteurs paient typiquement la valeur
nominale, les coupons réglant les intérêts. L'émetteur ajuste généralement
le taux de coupon au niveau du taux d'intérêt attendu par les acheteurs. Ce
taux fera que l'obligation vaut approximativement le nominal puisque chaque
coupon neutralise la croissance naturelle du capital.

Les obligations les plus liquides sont les obligations souveraines.
L'État français est un des plus gros émetteurs d'obligations du
monde, via ses 
[Obligations Assimilables du Trésor](https://www.aft.gouv.fr/fr/presentation-oat)
, ou OAT.

Les obligations sont dites assimilables parce que l'État continue d'émettre
des obligations selon les mêmes modalités que des émissions passées (même
maturité, même taux de coupon). Dans ce cas tous les titres sont fongibles.

Les émissions suivantes d'un même instrument se font à un prix dépendant du
taux d'emprunt du moment. Ainsi, certaines émissions se font au dessus du
pair, et d'autres sous le pair. L'Agence France Trésor rapporte le taux de
effectif moyen de chaque émission, paramètre le plus important pour évaluer
le coût de la dette.

### Valeur d'une obligation

Fondamentalement, une obligation est un flux de remboursements de petit
montant terminé par un remboursement de gros montant. Elle ressemble à
un crédit in fine avec quelques adaptations.

Les obligations (notamment souveraines) sont disponibles sur le marché
secondaire et soumises à
[cotation](https://live.euronext.com/en/product/bonds/fr001400fth3-motx).
Leur valeur est donnée en fraction du nominal (nommé *le pair*),
c'est-à-dire que le marché estime qu'elles valent plus ou moins cher selon
les coupons qu'elles servent.

Si une obligation se trouve *en dessous* du pair, c'est que le marché estime
qu'elle sert des coupons trop faibles pour « annuler » la croissance
naturelle du capital. À l'inverse, une obligation *au-dessus* du pair
signifie que le marché estime que les coupons sont trop élevés au
regard des taux d'intérêt demandés et donc qu'il faut payer plus cher pour
l'acquérir.

Si l'obligation est conservée jusqu'à maturité, le remboursement final est au
pair (pour les obligations standard) : on touche 1 € (ou la valeur nominale)
par unité d'obligation, ce qui clôt le contrat.

La valeur d'une obligation vaut donc la *valeur actuarielle nette* de
l'ensemble de ses flux (coupons et nominal à la fin) ajustés selon le taux
que le marché demande.

À l'inverse, on peut trouver le taux moyen de rendement d'une obligation en
équilibrant les flux par la méthode actuarielle entre les coupons et le nominal d'une part, et la valeur
constatée de l'obligation.

De ce fait, la valeur d'une obligation a un comportement un peu surprenant en
fonction de l'évolution des taux. Quand les taux augmentent, la valeur d'une
obligation donnée *diminue*. Inversement, quand les taux diminuent, sa valeur
*augmente*. Pour une maturité donnée, et pour un émetteur donné, le
marché a essentiellement un seul taux qui correspond au « risque » et toutes
les obligations se valent.

On pourra se reporter à l'excellent article de Claude Danthony
[Emprunts : mensualités, intérêt, taux, TEG, risque de taux](https://images.math.cnrs.fr/freeze/Emprunts-mensualites-interet-taux-TEG-risque-de-taux.html)
centré autour du crédit et qui comporte une section sur les obligations.

## Plan

La suite de la note sera consacrée à la fiscalité des obligations pour les
particuliers et abordera les points suivants :

- Principe de fiscalité : dispositions légales et comptabilité de caisse
- Exemples pratiques
- Analyse économique
- Analyse légale
- Effets macroéconomiques

## Principe de fiscalité

Pour les particuliers, les revenus des obligations se rangent dans la
catégorie des « revenus de capitaux mobiliers », dans la sous-catégorie «
produits de placement à revenu fixe ».

### Dispositions légales

Le Code général des impôts contient les dispositions suivantes pour le revenu des obligations :

- les articles [12 et 13](https://www.legifrance.gouv.fr/codes/section_lc/LEGITEXT000006069577/LEGISCTA000006179571) pour la définition du revenu
- les articles [118 et 119](https://www.legifrance.gouv.fr/codes/section_lc/LEGITEXT000006069577/LEGISCTA000006197365) pour le principe général de l'imposition sur les obligations
- l'article [125 A](https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000037526745) pour le prélèvement du revenu et le taux
- les articles [238 septies A à E](https://www.legifrance.gouv.fr/codes/section_lc/LEGITEXT000006069577/LEGISCTA000006179610) pour le cas des primes de remboursement,
  dont l'essentiel ne concerne pas / plus les personnes physiques.

Les BOFiPs relatifs aux obligations sont les suivants :

- [BOI-RPPM-RCM-20-10-20-20](https://bofip.impots.gouv.fr/bofip/929-PGP.html/identifiant=BOI-RPPM-RCM-20-10-20-20-20220630): règles générales d'assiette
- [BOI-RPPM-RCM-30-20](https://bofip.impots.gouv.fr/bofip/3774-PGP.html/identifiant=BOI-RPPM-RCM-30-20-20220630): prélèvement obligatoire pour les personnes physiques
    - [BOI-RPPM-RCM-30-20-10](https://bofip.impots.gouv.fr/bofip/3747-PGP.html/identifiant=BOI-RPPM-RCM-30-20-10-20210706): champ d'application
    - [BOI-RPPM-RCM-30-20-20](https://bofip.impots.gouv.fr/bofip/3740-PGP.html/identifiant=BOI-RPPM-RCM-30-20-20-20191220): recouvrement, dont prélèvements sociaux
    - [BOI-RPPM-RCM-30-20-30](https://bofip.impots.gouv.fr/bofip/3742-PGP.html/identifiant=BOI-RPPM-RCM-30-20-30-20230515): règles d'assiette
    - [BOI-RPPM-RCM-30-20-40](https://bofip.impots.gouv.fr/bofip/3748-PGP.html/identifiant=BOI-RPPM-RCM-30-20-40-20220630): taux

### Comptabilité de caisse

Le BOFiP BOI-RPPM-RCM-20-10-20-20 énonce les principes généraux
d'assiette pour les revenus de capitaux mobiliers.

Son point 1 reprend la lecture des articles 118 et 119 du CGI : s'entendent
donc taxables les intérêts et la prime de remboursement.

Le point 10 précise qu'il s'agit des « intérêt[s] et revenu[s] effectivement
perçu[s] au cours de l'année ».

Le reste du bulletin consiste en une discussion sur
la définition de la prime de remboursement, telle que définie sommairement
au 118 et 119 du CGI.

Une fois déterminés les principes de taxation, le recouvrement est organisé
de la façon suivante :

Le CGI dispose de la mise en œuvre du recouvrement, pour ce qui est des
personnes physiques par son article 125 A. La doctrine correspondante est le
bulletin BOI-RPPM-RCM-30-20.

On notera notamment dans la partie relative à l'assiette
(BOI-RPPM-RCM-30-20-30 § 20) que le montant brut du produit [de
l'obligation] est à considérer, sans retraitement.

Sans jamais définir précisément ce qui est de l'ordre du revenu,
un faisceau d'indices dans la doctrine nous laisse entendre que dans les faits
les organismes déclarateurs et collecteurs (c'est-à-dire les courtiers) sont
tenus d'appliquer une comptabilité stricte de caisse. Ainsi, chaque coupon
de l'obligation sera considéré en sa totalité comme du revenu. Pour ce qui
est du remboursement final il sera déduit le prix d'acquisition moyen
pondéré (incluant le coupon couru) afin déterminer la prime de remboursement.

Le reste de la note sera consacré à expliquer pourquoi cette assimilation de
l'entièreté du coupon à du revenu conduit à un problème de cohérence entre
assiette imposable et revenu économique dans certains exemples réels.

## Exemples

Nous allons montrer par deux exemples les effets de la comptabilité de
caisse en prenant deux obligations à maturité extrêmement proche (fin 2032)
mais servant des taux de coupon significativement différents (2% et 5,75%).
Nous simulons un investissement initial proche de 10 000€ et utilisons un
courtier facturant 0,2% de commission. Le cours retenu est celui à la
clôture sur le MOT le 23 avril 2026. Les obligations sont conservées jusqu'à
maturité.

Pour chacun des deux cas le revenu économique de l'opération dans sa
globalité sera calculé et comparé à l'assiette fiscale.

### Obligation sous le pair

Instrument : [OAT 2,00 % 25 novembre 2032](https://www.aft.gouv.fr/fr/titre/fr0000187635)

| Caractéristique | Valeur |
| --------------- | ------ |
| Coupon | 2% |
| Nominal | 1 € |
| Date d'achat | 2026-04-23 |
| Cours | 92,53% |
| Taux coupon couru | 0,99726% |
| Quantité | 10 671 |
| Prix brut | 9 873,88 € |
| Coupon couru | 106,42 € |
| Courtage | 19,75 € |
| Total acquisition | 10 000,05 € |
| Valeur du coupon | 213,42 € |


L'ensemble des flux comptables de l'opération s'échelonnent de la façon
suivante :

| Date | Flux | Assiette fiscale | Note |
| ---- | ---- | ---------------- | ---- |
| 2026-04-23 | -10 000,05 € || Acquisition |
| 2026-10-25 | 213,42 € | 213,42 € ||
| 2027-10-25 | 213,42 € | 213,42 € ||
| 2028-10-25 | 213,42 € | 213,42 € ||
| 2029-10-25 | 213,42 € | 213,42 € ||
| 2030-10-25 | 213,42 € | 213,42 € ||
| 2031-10-25 | 213,42 € | 213,42 € ||
| 2032-10-25 | 213,42 € | 213,42 € ||
| 2032-10-25 | 10 671,00 € | 670,95 € | Prime de remboursement |
|||||
| Taux de rendement interne | 3,25% |||
| Enrichissement | 2 164,89 € |||
| Assiette fiscale | 2 164,89 € |||


Du fait de la décote à l'acquisition une comptabilité de caisse ne pose pas
de problème. Chaque coupon peut être considéré comme un enrichissement à
part entière, la prime de remboursement, positive dans ce cas est aussi
rapportée à l'assiette.

Économiquement cette prime peut être analysée comme des intérêts latents accumulés dans
le capital restant dû (au taux de rendement interne) et dont le solde a lieu au remboursement.

### Obligation au dessus du pair

Instrument : [OAT 5,75 % 25 octobre 2032](https://www.aft.gouv.fr/fr/titre/fr0000187635)

Cette obligation crée au début des années 2000 s'échange systématiquement
au dessus du pair depuis de nombreuses années, y compris lors des
adjudications ayant eu lieu ultérieuement par l'Agence France Trésor.

| Caractéristique | Valeur |
| --------------- | ------ |
| Coupon | 5,75% |
| Nominal | 1 € |
| Date d'achat | 2026-04-23 |
| Cours | 114,45% |
| Taux coupon couru | 2.8671% |
| Quantité | 8 507 |
| Prix brut | 9 736,26 € |
| Coupon couru | 243,91 € |
| Courtage | 19,47 € |
| Total acquisition | 9 999,64 € |
| Valeur du coupon | 489,15 € |


L'ensemble des flux comptables de l'opération s'échelonnent de la façon
suivante :

| Date | Flux | Assiette fiscale | Note |
| ---- | ---- | ---------------- | ---- |
| 2026-04-23 | -9 999,64 € || Acquisition |
| 2026-10-25 | 489,15 € | 489,15 € ||
| 2027-10-25 | 489,15 € | 489,15 € ||
| 2028-10-25 | 489,15 € | 489,15 € ||
| 2029-10-25 | 489,15 € | 489,15 € ||
| 2030-10-25 | 489,15 € | 489,15 € ||
| 2031-10-25 | 489,15 € | 489,15 € ||
| 2032-10-25 | 489,15 € | 489,15 € ||
| 2032-10-25 | 8 507 € | -489,15 € | Déficit fiscal sec |
|||||
| Taux de rendement interne | 3,20% |||
| Enrichissement | 1 931,43 € |||
| Assiette fiscale | 2 934,92 € || !!!! |


La doctrine permet d'imputer la perte au remboursement sur le dernier coupon
BOI-RPPM-RCM-20-10-20-20 § 390

Du fait de la comptabilité en caisse stricte, la dernière année implique un
montant rapportable de 0€.

Par la définition extrêmement stricte de revenu fiscal, la doctrine induit
une inflation d'assiette *d'environ 50% comparé au strict enrichissement*.

Dans ces conditions il est difficile de concilier l'assiette fiscale avec la
notion de revenu.

## Analyse économique des obligations en surcote ou en décote

### Méthode actuarielle

Nous allons tenter une analyse économique de l'effet d'une décote ou d'une
surcote d'une obligation.

Un outil essentiel en analyse économique pour caractériser des flux
financiers est le taux de rendement interne. Il est défini comme le taux `t`
qui égalise les flux par la méthode actuarielle.

Ainsi pour une obligation achetée à une certaine fraction `P` du pair, qui
verse des coupons `C` (exprimé en fraction du pair), sur `n` annuités et
qui rembourse `R` à la fin, le taux de rendement interne `t`
sera défini par la formule :

<!-- p = \sum_{i = 1}^{n} \frac{C}{(1+t)^i} + \frac{r}{(1+t)^n} -->
<!-- https://temml.org/ -->

<math display="block" class="tml-display" style="display:block math;">
  <mrow>
    <mi>P</mi>
    <mo>=</mo>
    <mrow>
      <munderover>
        <mo movablelimits="false">∑</mo>
        <mrow>
          <mi>i</mi>
          <mo>=</mo>
          <mn>1</mn>
        </mrow>
        <mi>n</mi>
      </munderover>
    </mrow>
    <mfrac>
      <mi>C</mi>
      <msup>
        <mrow>
          <mo fence="true" form="prefix" stretchy="false">(</mo>
          <mn>1</mn>
          <mo>+</mo>
          <mi>t</mi>
          <mo fence="true" form="postfix" stretchy="false">)</mo>
        </mrow>
        <mi>i</mi>
      </msup>
    </mfrac>
    <mo>+</mo>
    <mfrac>
      <mi>R</mi>
      <msup>
        <mrow>
          <mo fence="true" form="prefix" stretchy="false">(</mo>
          <mn>1</mn>
          <mo>+</mo>
          <mi>t</mi>
          <mo fence="true" form="postfix" stretchy="false">)</mo>
        </mrow>
        <mi>n</mi>
      </msup>
    </mfrac>
  </mrow>
</math>

Cette formule se simplifie en :

<!-- P = \frac{C}{t}\left[1 - \frac{1}{(1+t)^n} \right] + \frac{r}{(1+t)^n} -->

<math display="block" class="tml-display" style="display:block math;">
  <mrow>
    <mi>P</mi>
    <mo>=</mo>
    <mfrac>
      <mi>C</mi>
      <mi>t</mi>
    </mfrac>
    <mrow>
      <mo fence="true" form="prefix" stretchy="true">[</mo>
      <mn>1</mn>
      <mo>−</mo>
      <mfrac>
        <mn>1</mn>
        <msup>
          <mrow>
            <mo fence="true" form="prefix" stretchy="false">(</mo>
            <mn>1</mn>
            <mo>+</mo>
            <mi>t</mi>
            <mo fence="true" form="postfix" stretchy="false">)</mo>
          </mrow>
          <mi>n</mi>
        </msup>
      </mfrac>
      <mo fence="true" form="postfix" stretchy="true">]</mo>
    </mrow>
    <mo>+</mo>
    <mfrac>
      <mi>R</mi>
      <msup>
        <mrow>
          <mo fence="true" form="prefix" stretchy="false">(</mo>
          <mn>1</mn>
          <mo>+</mo>
          <mi>t</mi>
          <mo fence="true" form="postfix" stretchy="false">)</mo>
        </mrow>
        <mi>n</mi>
      </msup>
    </mfrac>
  </mrow>
</math>

C'est ce taux `t` qui est publié par l'Agence France Trésor suite à chaque
émission obligataire, dans le cas des emprunts d'État.

Quand `R` est égal à `0` et `P` est égal à `1` on retrouve la formule du crédit
amortissable où tout le capital est amorti en cours de route et il ne reste
plus rien à solder à la fin. Certaines obligations dites « amortissables »
sont sous ce format, typiquement pour du financement d'infrastructures.

Quand `R = 1` et `P = 1`, on retrouve l'obligation classique au moment de
son émission initiale en syndication, où l'émetteur ajuste son taux de
coupon au taux d'intérêt demandé par le marché.

Quand `R = 1` et `P ≠ 1` on tombe sur les scénarios intermédiaires des
obligations trouvées sur le marché secondaire ou négociées lors des
adjudications supplémentaires.

Une obligation, du point de vue de l'acheteur, ce n'est ni plus ni moins
qu'un contrat de crédit in fine, avec paiement d'un ballon.

La formule se simplifie à `C = t` quand l'obligation est cotée au pair, ie `P`
est égal à `1`.

Au sens économique du terme, l'enrichissement économique est la somme des
coupons, plus le remboursement moins la mise de départ. Mais c'est aussi,
dans le cas d'un crédit, égal aux intérêts générés. Il est possible de
les calculer de la manière suivante :

### Calcul des intérêts

Dans un crédit, les intérêts facturés à chaque période sont égaux au capital
restant dû à la période précédente multiplié par le taux d'intérêt.

Dans notre cas, le taux de rendement interne `t` ayant été déterminé à
l'achat (il dépend notamment du coupon `C`, du nombre d'annuités `n`, et du prix payé
`P`), le capital restant dû à l'étape `k` vaut la valeur actuarielle nette
des flux à venir sous ce taux d'actualisation. Ainsi, pour un remboursement au pair,
on peut montrer que :

<math display="block" class="tml-display" style="display:block math;">
  <mrow>
    <mi>C</mi>
    <mi>R</mi>
    <msub>
      <mi>D</mi>
      <mrow>
        <mi>k</mi>
      </mrow>
    </msub>
    <mo>=</mo>
    <mfrac>
      <mi>C</mi>
      <mi>t</mi>
    </mfrac>
    <mrow>
      <mo fence="true" form="prefix" stretchy="true">[</mo>
      <mn>1</mn>
      <mo>−</mo>
      <mfrac>
        <mn>1</mn>
        <msup>
          <mrow>
            <mo fence="true" form="prefix" stretchy="false">(</mo>
            <mn>1</mn>
            <mo>+</mo>
            <mi>t</mi>
            <mo fence="true" form="postfix" stretchy="false">)</mo>
          </mrow>
          <mrow>
            <mi>n</mi>
            <mo>−</mo>
            <mi>k</mi>
          </mrow>
        </msup>
      </mfrac>
      <mo fence="true" form="postfix" stretchy="true">]</mo>
    </mrow>
    <mo>+</mo>
    <mfrac>
      <mn>1</mn>
      <msup>
        <mrow>
          <mo fence="true" form="prefix" stretchy="false">(</mo>
          <mn>1</mn>
          <mo>+</mo>
          <mi>t</mi>
          <mo fence="true" form="postfix" stretchy="false">)</mo>
        </mrow>
        <mrow>
          <mi>n</mi>
          <mo>−</mo>
          <mi>k</mi>
          </mrow>
        </mrow>
      </msup>
    </mfrac>
  </mrow>
</math>

On notera que cette formule donne par construction exactement le prix payé `P`
quand `k = 0`; et `1`, soit le pair, quand `k = n`.

Les intérêts dus à l'annuité `k` valent donc :

<math display="block" class="tml-display" style="display:block math;"><mrow><msub><mi>I</mi><mi>k</mi></msub><mo>=</mo><mi>C</mi><mi>R</mi><msub><mi>D</mi><mrow><mi>k</mi><mo>−</mo><mn>1</mn></mrow></msub><mo>⋅</mo><mi>t</mi></mrow></math>

Et enfin nous obtenons la part d'amortissement :

<math display="block" class="tml-display" style="display:block math;"><mrow><msub><mi>A</mi><mi>k</mi></msub><mo>=</mo><mi>C</mi><mo>−</mo><msub><mi>I</mi><mi>k</mi></msub></mrow></math>

#### Obligation en surcote

L'obligation en surcote se traduit mathématiquement par un taux de rendement
interne inférieur au coupon : `t < C`. Dans ces conditions la part de capital
rendue `Ak` est généralement positive. Dit autrement la perte constatée au
remboursement (car le prix payé `P` est supérieur au pair) correspond en
fait à un retour économique de capital en cours de route via les coupons.

Une autre façon de le voir est que si les coupons étaient strictement du
revenu, le récipiendaire pourrait les consommer sans toucher au capital. Or
ici nous avons une différence entre le prix payé pour l'acquisition du
contrat et le remboursement au pair. Cette différence trouve sa
contrepartie dans les coupons et la consommation des coupons dans leur
entièreté revient à amputer une partie de capital.

C'est à ce stade que la simplification administrative devient discutable :
elle assimile à un revenu l'intégralité d'un flux (les coupons `C`) dont
seulement une partie correspond économiquement à des intérêts, l'autre étant
une restitution de capital.

On pourra retrouver [le tableau d'amortissement en annexe](annexe_tableau_amortissement.md)
pour l'exemple acheté en surcote qui détaille la part de capital et
d'intérêt de chaque coupon comme déterminé par la méthode actuarielle.

#### Obligation en décote

De manière symétrique, quand l'obligation est achetée sous le pair (`P < 1`
ce qui provoque un taux `t > C`), le capital restant dû accumule
silencieusement des intérêts, qui se trouvent soldés sous la forme de prime
de remboursement.  Dans ce cas la simplification administrative reste
cohérente puisque la prime de remboursement est de signe positive et peut
être incluse dans une assiette taxable, les coupons n'étant composés que
d'intérêts.

### Remarque sur la méthode actuarielle

Cette méthode actuarielle n'est pas la seule méthode possible pour ventiler
la part des intérêts d'un crédit, mais elle est pertinente comme outil d'analyse
pour au moins trois raisons :

- elle permet d'assigner un taux d'intérêt naturel au contrat en
  l'assimilant à un crédit classique ce qui permet d'identifier la part
  d'intérêts vs capital pour chaque flux d'argent, tout en gardant *par
  construction* qu'en fin de parcours la somme des intérêts calculés est
  strictement égale à l'enrichissement économique.
- elle permet de suivre la valeur de revient de l'obligation au fil du
  temps, en partant du prix d'acquisition et en tenant compte des coupons déjà
  servis selon une logique actuarielle. Cette valeur n'est pas un prix de
  marché aux taux courants, mais la valeur de revient du capital encore immobilisé
  selon les paramètres déterminés au moment de l'achat.
- cette méthode est déjà connue du code général des impôts. Ainsi, pour les
  personnes morales détentrices d'obligations, les articles 238 septies A à E
  du CGI disposent dans certains cas l'usage de la méthode actuarielle afin
  d'inscrire au bilan les intérêts cachés des primes de remboursement.

Dans tous les cas, cette analyse permet de montrer que quand on assimile une
obligation à un contrat de crédit générant des intérêts, dans la logique de
des articles 118 et 119 du CGI qui visent les « intérêts et produits », les
flux d'argent servis peuvent comporter une partie d'intérêts et une partie
de capital.

## Analyse légale

La base légale de l'imposition des revenus de capitaux mobiliers et
notamment les placements à revenu fixe trouve sa source dans les articles 12
et 13 du CGI, précisé par les articles 118 et 119 pour ce qui concerne les
obligations et autres produits assimilés.

Ainsi pour être compris dans l'assiette imposable, il ne suffit pas qu'un flux
d'argent provienne d'une obligation. Encore faut-il qu'il puisse être qualifié d'«
intérêts » , « arrérage »  ou de « produit ». Le traitement des primes de
remboursement illustre bien cette logique : le remboursement final n'est pas
taxable en tant que tel; seule la fraction excedant le capital restitué est
suceptible d'être qualifié de produit imposable.

La doctrine concernant les revenus de capitaux mobiliers, notamment le bulletin
BOI-RPPM-RCM-20-10-20-20 opère un probable glissement entre coupons d'une
obligation et intérêt, sans toutefois jamais le dire explicitement : le bulletin
ne contient aucune occurence du mot coupon, alors que ce terme est d'usage
en finance. La doctrine se contente de parler d'intérêts et de produits. On
pourra notamment relever le §380 traitant le cas de la perte au
remboursement où l'assimilation entre coupons et intérêts apparaît le plus
clairement.

Une fois réalisé ce glissement, le recouvrement pour les particuliers,
traité par le bulletin BOI-RPPM-RCM-30-20, conclue logiquement à la règle de
comptabilité de caisse : un coupon est un revenu, et son montant brut est
à inclure dans l'assiette taxable. On notera que l'article 125 A dont le
bulletin assure la mise en œuvre vise lui aussi le revenu brut.  Cette
précision ne tranche cependant pas la qualification préalable du flux.
Elle peut être comprise comme excluant la déduction de frais ou commissions
afférants à la perception du revenu (typiquement commissions d'arrérages);
elle n'implique pas nécéssairement que tout flux encaissé doive être
qualifié de revenu dans son intégralité.

Or, nous avons vu par les analyses développées dans cette note que le marché
des obligations, qu'il soit primaire ou secondaire n'utilise pas la
qualification des flux afin de déterminer un prix. Seule compte la valeur
actuarielle nette des flux. Dans ce cadre tout mouvement d'argent est traîté
de manière neutre.

Il est de notre avis que la fiscalité ne devrait pas s'arrêter aux
qualifications contractuelles pour déterminer ce qui constitue un revenu
mais aussi considérer le point de vue de la personne qui s'enrichit et qui
reçoit une suite de flux monétaires en échange d'un paiement initial. 

De fait, du point de vue de l'acheteur qui s'enrichit, il n'y a aucune
différence en terme de flux stricts entre une obligation et un contrat de
crédit qui contiendrait un tableau d'amortissement libellant intérêts et
retour de capital, et reproduisant exactement les flux économiques d'une
obligation.

Considérant que le code des impôts se contente de rester en termes généraux
et laisse la pratique définir ce qu'est un revenu, il est possible de penser
que l'interprétation qu'en prend l'administration est une opinion qui n'a
pas été formulée explicitement par le législateur.

Ainsi, la doctrine, en appliquant une comptabilité de caisse stricte et en
assimilant les coupons à du revenu dans leur entièreté opère une
simplification d'ordre administrative.

Dans le cas des obligations achetées sous le pair cette simplification ne
pose pas de problème, les intérêts cachés non réglés par les coupons se
retrouvent soldés dans la prime de remboursement. C'est ici que les articles
238 septies A à E du CGI entrent en jeu afin de rajouter de l'assiette en
avance de phase, pour les personnes morales. Pour le cas des personnes
physiques le législateur considère, à raison, que ces intérêts cachés
n'ayant pas été touchés ils sont logiquement à traîter au niveau de la prime
de remboursement.

Dans le cas des obligations achetés au dessus du pair, cette simplification
administrative ne fonctionne plus et finit par créer une base taxable qui
s'éloigne de la notion de revenu économique et dépasse probablement
l'intention du législateur. De fait, nous montrons qu'une analyse plus fine,
déjà connue du législateur et des normes comptables internationales permet de
bien séparer du point de vue du contribuable détenteur de l'obligation, ce
qui est intérêts vs retour de capital, pour chaque flux élementaire du
contrat.

La situation est encore pire avec une obligation amortissable, l'État
français n'en émet pas mais c'est un mode typique de financement pour les
infrastructures. Dans ces conditions l'ensemble du contrat est prévu pour
s'amortir en cours de vie, il n'y a pas de ballon. La simplification conduirait
à identifier l'entièreté des flux comme des intérêts et donc taxer aussi
la mise de départ comme s'il s'agissait de revenu.

Dès lors, il est raisonnable de penser qu'en interdisant de tenir compte de la
perte au remboursement, tout en reconnaissant qu'elle trouve sa contrepartie
dans les coupons, la doctrine commet une *erreur de qualification* de ces
coupons en les déclarant intérêts (donc revenus) alors qu'une fraction est
identifiable comme un remboursement de capital.

Par ailleurs, il nous semble qu'en raison du principe de neutralité fiscale
il ne devrait pas y avoir une telle distorsion d'assiette entre revenu
fiscal et revenu économique en fonction des paramètres internes des
instruments d'un même émetteur au revenu économique rendement interne et
maturités similaires.

Dans le cas d'espèce, l'exemple cité plus haut ayant une inflation de
l'assiette fiscale de 50% par rapport au revenu économique semble dépasser
largement ce qui peut être attendu des effets d'une simplification
administrative.

Notons que le code général des impôts dans ses articles fondateurs et
générateurs du fait taxable que sont les articles 12, 13, 118 et 119, ne
fait pas de différence entre la qualité des personnes qui touchent les
revenus, pour ce qui est de la définition même de l'assiette taxable.
Tandis qu'il est tout à fait normal que les règles de liquidation, de taux,
d'abattement etc varient selon qu'il s'agisse d'une personne physique ou d'une
personne morale, il nous semble difficile de justifier que certaines personnes
morales, selon leur référentiel comptable puissent inscrire en charge
l'amortissement des surcotes des obligations alors que les particuliers ne
puissent pas le faire ce faisant introduisant une difficulté vis-à-vis des
principes généraux d'égalité devant l'impôt.

Enfin, du fait des mécanismes d'attraction vers le pair de la valeur des
obligations au fur et à mesure de l'approche de l'échéance du remboursement
(voir l'analyse économique), pour le cas des obligations liquides, le
contribuable à qui on a imposé une comptabilité de caisse pour une
obligation en surcote pourra revendre l'instrument peu de temps avant
l'échéance pour bénéficier des mécanismes de report en moins-value en
application des articles 150-0 A et suivants du CGI. Il ne nous semble pas
pertinent que la doctrine encourage de fait ce genre de comportement
uniquement à visée fiscale et ce pour les raisons suivantes :

- l'application du 150-0 D du CGI dépend de la vente effective et donc de
  l'existence d'une contrepartie pour acheter l'instrument, de ce fait
  avantageant les obligations liquides, ce qui constitue un problème de
  neutralité fiscale;
- il s'agit d'un détournement sans raison économique de cette passerelle
  prévue pour les aléas de marché afin de palier à une situation pourtant
  prévisible dès le départ, ce faisant elle expose le contribuable à un risque
  de qualification d'abus de droit;
- et globalement pose un problème de cohérence car elle nécéssite que le
  contribuable ait des plus values à effacer dans cette catégorie de
  revenus. Or il nous semble que l'imposition devrait être autoporteuse, le
  problème se situe au niveau des produits de placement à revenu fixe, la
  doctrine devrait proposer une solution viable dans cette catégorie.

## Effets macroéconomiques

[à ajouter]

## Note conclusive

Le CGI pose comme principe d'imposer intérêts et produits sans donner précisément
leur définition. Les obligations sont des contrats qui génèrent des flux
économiques (série de coupons et remboursement final au pair), négociables
sur le marché secondaire. Selon les cas, une fraction des coupons peut ne pas
être considérée comme un revenu économique (viz. IFRS 9 §5.4.1).
Néanmoins par simplification la doctrine considère dans le cas
des personnes physiques l'entièreté des coupons comme un revenu au plan
fiscal et ce faisant commet une erreur de qualification du revenu. Cela
provoque un différentiel notable entre revenu fiscal et revenu économique
dans le cas d'une acquisition du contrat au-dessus du pair sur le marché
secondaire.

Cette situation est reconnue par les points 380 et 390 du bulletin BOI-RPPM-RCM-20-10-20-20,
qui proposent une solution ad hoc de compensation du dernier coupon pour
adoucir la situation d'une prime de remboursement négative. Cette solution
est insuffisante et ne permet pas d'éviter des différentiels d'assiette très
importants, dépassant ce qu'on peut raisonnablement attendre d'une
simplification pour des raisons de gestion administrative. Notamment cela
conduit à taxer très différemment les produits d'instruments considérés
pourtant équivalents du point de vue actuariel (taux de rendement interne
similaire, enrichissement net similaire).

En soi, une comptabilité de caisse n'est pas forcément incompatible avec le
cas d'une obligation achetée avec surcote et gardée à maturité. Cependant, en
refusant de proposer un mécanisme permettant d'aligner revenu fiscal et
revenu économique, la doctrine s'est retrouvée à dépasser l'intention du législateur
de taxer uniquement les revenus en assimilant la totalité des coupons à des
intérêts alors qu'une analyse économique reconnue permet d'identifier une
partie des flux comme un retour de capital et l'autre comme des intérêts.

Enfin, cette situation incite à des comportements non économiques pour des
raisons fiscales : revente en fin de remboursement afin de générer une moins-value
reportable, sans raison économique sous-jacente.
