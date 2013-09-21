#Présentation des tests logiciels

Cet article est le premier d'une série sur les tests logiciels.
A travers cette série, nous définirions l'utilité des tests logiciels, les différents types de tests ainsi que la méthodologie permettant de les mettre en place.

##Utilité des tests logiciels

###Contexte

Les systèmes logiciels font désormais partie intégrante de la vie de tous, que soit des applications utilisées dans les entreprises au plus simple produit de consommation.

Et la plupart des gens ont connu une expérience avec une application qui ne fonctionne pas comme prévu.  
Ces dysfonctionnements entrainent indubitablement de plus gros problèmes, comme la perte d'argent, de temps ou de réputation de l'entreprise.

###Origine des défauts logiciels

Les êtres humains font des erreurs. Les développeurs font donc des erreurs.  
Ces erreurs produisent un défaut (panne, bug) dans le code du programme ou dans un document. 
Si un code défectueux est exécuté, le système risque d'échoué dans ce qu'il doit faire, (ou faire quelque chose qu'il ne devrait pas), entraînant une panne.

Les défauts apparaissent parce que les êtres humains sont faillibles mais aussi par divers facteurs :

- la pression du temps,

- le changement,

- la complexité du code,

- la complexité de l'infrastructure, 

- l'évolution des technologies 

- les interactions entre de nombreux systèmes...

### Rôle des tests dans le développement et la maintenance logiciel.

Des tests rigoureux effectués sur les applications et sur la documentation peuvent aider à réduire le risque de disfonctionnement et ainsi contribuer à la qualité du logiciel, si les défauts constatés sont corrigés avant que le système soit mis en production.

Les tests logiciels peuvent également être nécessaires pour répondre à des exigences contractuelles ou légales, ou à des normes spécifiques de l'industrie.

###Tests et qualité

A l'aide de tests, il est possible de mesurer la qualité des logiciels pour les exigences fonctionnelles et non fonctionnelles  du logiciel ainsi que ses caractéristiques (par exemple, la fiabilité, la convivialité, l'efficacité, la maintenabilité et la portabilité…)

Des leçons doivent être tirées des projets antérieurs. En comprenant les causes profondes des défauts
trouvés dans d'autres projets, les processus peuvent être améliorés, ce qui devrait limiter la récurrence des 

défauts et, par conséquent, améliorer la qualité des applications futures.

Il s'agit d'un aspect de l'assurance qualité. Le test doit donc être intégré comme l'une des activités de 

l'assurance qualité (c.-à-d. parallèlement au développement).

###Combien de tests sont suffisants? 

La granularité des tests doit tenir compte du niveau de risque, technique et stratégique, ainsi que des contraintes liées au projet telles que le temps et le budget. 
Les tests doivent fournir des informations suffisantes pour aider les parties prenantes à prendre des décisions éclairées. 

##Définitions

Deux entités régissent les tests logiciels : l'ISTQB (International  Software  Testing Qualifications  Board) et le CFTL (Comité Français des Tests Logiciels)

###Test [ISTQB]

Processus consistant en toutes les activités du cycle de vie, statiques et dynamiques, concernant la planification et l’évaluation de produits logiciels et produits liés pour déterminer s’ils satisfont aux exigences, pour démontrer qu’ils sont aptes au objectifs et détecter des anomalies.

###Test [IEEE-829-2008]

Un test est un ensemble de cas à tester (état de l'objet à tester avant exécution du test, actions ou données en entrée, valeurs ou observations attendues, et état de l'objet après exécution), éventuellement accompagné d'une procédure d'exécution (séquence d'actions à exécuter). Il est lié à un objectif.  
Un test vise à mettre en évidence des défauts de l'objet testé. Cependant il n'a pas pour objectif :

- de diagnostiquer la cause des erreurs
- de les corriger
- de prouver la correction de l'objet testé.

### Suite de tests

Un ensemble de plusieurs cas de tests pour un composant ou système sous test, où les post-conditions d’un test sont souvent utilisées comme pré-conditions du test suivant.

## Principes

Un certain nombre de principes de test ont été suggérés pendant les 40 dernières années et offrent des lignes directrices communes pour tous les tests.

###Les tests montrent la présence de défauts

Les tests peuvent prouver la présence de défauts, mais ne peuvent pas prouver qu'il n'existe pas de défauts.  
Tester un logiciel réduit la probabilité d'apparition de défauts, mais, même si aucun défaut n'a été trouvé, cela ne constitue pas une preuve d'absence de défauts.

###L'exhaustivité des tests est impossible

Tout tester (toutes les combinaisons d'entrants et des conditions) n'est pas possible sauf pour les cas triviaux.  
A la place de tests exhaustifs, l'analyse des risques et des priorités devrait être utilisé pour définir les tests.

###La précocité des tests

Les activités de test doivent commencer le plus tôt possible dans le cycle de développement et doivent être axés sur des objectifs définis.

### Partitionnement des défauts

L'effort de test doit être porté proportionnellement à la densité de défauts attendu et observé par modules.  
Un petit nombre de modules contient généralement la plupart des défauts détectés au cours des tests préliminaires ou est responsable de la plupart des pannes de fonctionnement.

###Le "paradoxe des pesticides"

Si les mêmes tests sont répétés maintes et maintes fois, il se peut que le même ensemble de tests ne puisse plus trouver de nouveaux défauts. Pour surmonter ce "paradoxe de pesticides", les cas de test doivent être régulièrement examiné et révisé, et de nouveaux tests doivent être écrits afin de trouver d'autres défauts.

###Les tests sont dépendants du contexte 

Les tests doivent être adaptés à leurs contextes. 

### L'illusion de l'absence d'erreurs

Trouver et corriger des défauts n'apporte rien si le logiciel développé est inutilisable ou ne remplit pas les besoins et les attentes des utilisateurs.

## Classifications des tests logiciels
### Les niveaux de test
#### Tests de composants (tests unitaires)
#### Tests d'intégration
#### Tests système
#### Tests d'acceptation

### Les types de tests

### Les catégories de tests

## Autres généralités sur les tests logiciels
