# Exemple d'amortissement d'une obligation en surcote

Pour rappel, l'obligation achetée en surcote correspond aux paramètres
suivants. Le cours a été pris à la clôture au MOT au 23 avril 2026 et les
frais de courtage ont été fixés à 0,2% :

Instrument : [OAT 5,75 % 25 octobre 2032](https://www.aft.gouv.fr/fr/titre/fr0000187635)

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


Nous utilisons la méthode actuarielle pour ventiler chaque flux entre
intérêts et amortissement de capital. Le taux de rendement interne capture
exactement le taux effectif qu'il faut considérer pour que les flux
ressemblent à un contrat de crédit classique où le capital est augmenté des
intérêts à chaque période, puis amputé du remboursement.

| Date       | Flux        | Part intérêts | Part capital | CRD         |
| ---------- | ----------- | ------------- | ------------ | ----------- |
| 2026-04-23 | -9 999,64 € |           0 € |  -9 999,64 € | -9 999,64 € |
| 2026-10-25 |    489,15 € |      161,07 € |     328,09 € | -9 671,55 € |
| 2027-10-25 |    489,15 € |      309,76 € |     179,39 € | -9 492,16 € |
| 2028-10-25 |    489,15 € |      304,86 € |     184,29 € | -9 307,88 € |
| 2029-10-25 |    489,15 € |      298,11 € |     191,04 € | -9 116,84 € |
| 2030-10-25 |    489,15 € |      292,00 € |     197,16 € | -8 919,68 € |
| 2031-10-25 |    489,15 € |      285,68 € |     203,47 € | -8 716,21 € |
| 2032-10-25 |    489,15 € |      279,94 € |     209,21 € | -8 507,00 € |
| 2032-10-25 |     8 507 € |        0,00 € |   8 507,00 € |      0,00 € |
||||||
| Taux de rendement interne | 3,20% ||||
| Enrichissement net | 1 931,34 € ||||
| Total intérêts | 1 931,34 € ||||

Le taux de rendement interne a été déterminé par la formule d'équivalence
des flux. Ainsi *par construction* la méthode actuarielle assure l'égalité
entre la somme des intérêts et l'enrichissement net.

Le capital restant dû diminuant, la part d'intérêts perçue diminue, de la
même manière que dans un crédit amortissable classique. C'est exactement ce
mécanisme qui fait que pour les obligations le pair agit comme attracteur.

À noter qu'à cause de la non périodicité stricte des flux, le taux annuel a
été journalisé en méthode actuarielle, et une convention de calcul en jours
exacts a été utilisée pour le calcul des intérêts. Cela a pour conséquence
que le coupon couru réglé au moment de l'achat a été neutralisé dès le
premier versement, les intérêts n'ayant pas eu le temps de s'accumuler sur
une année entière. Cela nous semble cohérent avec une analyse en termes
de rendement strict du capital.

## Commentaire

La méthode actuarielle est un moyen courant d'analyse des contrats de type
crédit, et requise par la réglementation dans de nombreux cas (p.ex. pour ce
qui est des personnes physiques, par le calcul des TAEG).

La distorsion entre assiette fiscale et revenu économique justifie une
méthode plus fine qu'une comptabilité de caisse pure pour distinguer la part
des intérêts de la part de retour de capital, dans le cas des obligations
achetées au dessus du pair.

Dans le passé un tel type d'analyse aurait probablement demandé des moyens
jugés disproportionnés au regard des outils informatiques disponibles et des
taux souverains de l'époque, et pouvait justifier une comptabilité en
caisse. De nos jours l'ubiquité des ordinateurs et des modules d'analyse
financiers rend difficile une telle justification, notamment dans un univers
de taux relativement faibles qui exacerbe les effets des obligations
échangées au-dessus du pair.
