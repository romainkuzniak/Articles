#Présentation des tests logiciels

Cet article est le premier d'une série sur les tests logiciels.
A travers cette série, nous définirions l'utilité des tests logiciels, les différents types de tests ainsi que la méthodologie permettant de les mettre en place.

##Utilité des tests logiciels TODO

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

### Combien de tests sont suffisants? 

La granularité des tests doit tenir compte du niveau de risque, technique et stratégique, ainsi que des contraintes liées au projet telles que le temps et le budget. 
Les tests doivent fournir des informations suffisantes pour aider les parties prenantes à prendre des décisions éclairées. 

## Définitions des tests logiciels TODO

Deux entités régissent les tests logiciels : l'ISTQB (International  Software  Testing Qualifications  Board) et le CFTL (Comité Français des Tests Logiciels).  
Cependant, il existe une plethore de normes définissant les tests logiciels: 

- IEEE 829

- IEEE 1008

- BS 7925-1/ -2

- IEEE 1028

- ...  

La norme **ISO/IEC 29119** a pour objectif de les réunir.  

### Test [ISTQB]

Un ensemble de plusieurs cas de tests.

### Cas de tests [ISTQB / BS 7925-1]
Un ensemble d'entrées, de pré conditions d'execution, et de résultats attendus, développer pour un objectif précis comme éprouver un programme ou vérifier la comformité à des exigences particulières.

###Test [IEEE-829-2008]

Un test est un ensemble de cas à tester (état de l'objet à tester avant exécution du test, actions ou données en entrée, valeurs ou observations attendues, et état de l'objet après exécution), éventuellement accompagné d'une procédure d'exécution (séquence d'actions à exécuter). Il est lié à un objectif.  
Un test vise à mettre en évidence des défauts de l'objet testé. Cependant il n'a pas pour objectif :

- de diagnostiquer la cause des erreurs
- de les corriger
- de prouver la correction de l'objet testé.

### Suite de tests [ISTQB]

Un ensemble de plusieurs cas de tests pour un composant ou système sous test, où les post-conditions d’un test sont souvent utilisées comme pré-conditions du test suivant.

## Principes des tests logiciels

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
Il existe plusieurs niveaux de tests :

- Les tests de composants (ou tests unitaires)
- Les tests d'intégration
- Les tests système
- Les tests d'acceptation

#### Test de composants (test unitaire)

##### Définitions

- Composant : un élément logiciel minimal qui peut être testé isolément.
- Test de composant : le test de composants logiciels individuels [d’après IEEE 610]

Les tests de composants (également connu comme tests unitaires, tests de module ou tests de programme) vérifient le fonctionnement des modules logiciels, des programmes, des objets, des classes, etc
Ils peuvent être réalisés indépendamment du reste du système.

##### Elements servant de base de test :
- les stories
- Le code source
- les exigences de composants
- la conception technique détaillée

Objets de test typique :

- Des composants (classes, méthodes ...)
- Programmes
- Conversion de données des programmes / migration
- Modules de base de données

#### Test d'intégration

##### Définitions

- Tests d’intégration : tests effectués pour montrer des défauts dans les interfaces et interactions des composants ou des systèmes intégrés.
- Intégration : le processus de combiner des composants ou des systèmes en assemblages plus grands.

Les tests d'Intégration testent les interfaces entre les composants, les interactions entre les différentes parties d'un système, tels que le système d'exploitation, le système de fichiers, le matériel, et les interfaces entre les systèmes.

##### Base de test:

- Logiciel et conception des systèmes
- Architecture
- Workflows
- Cas d'utilisation

Objets de test typique :
- Implémentation de sous-systèmes de base de données
- Infrastructure
- Interfaces
- Les données de configuration

#### Test système

##### Définitions
- Système : une collection de composants organisés pour accomplir une fonction ou un ensemble de fonctions spécifiques [IEEE 610]
- Tests système : le processus de test d’un système intégré pour vérifier qu’il réponde à des exigences spécifiques [Hetzel]

Les tests système prennent en compte le comportement de l'intégralité d'un système. La portée des tests doit être clairement abordée dans le plan de test.  L'environnement de test doit correspondre à l'environnement production final autant que possible afin de minimiser le risque de défaillances spécifiques à l'environnement de test.

##### Base de test:
- Système et spécification des besoins du logiciel
- Cas d'utilisation
- Spécifications fonctionnelles
- Les rapports d'analyse des risques

##### Objets de test typique:
- Manuels d'utilisation, de fonctionnement et du système
- Configuration du système
- Données de configuration

### Tests d'acceptation

##### Définitions
- Critère d’acceptation : le critère de sortie que doit satisfaire un composant ou un système de façon à être accepté par un utilisateur, client ou une autre entité autorisée [IEEE 610]
- Test d’acceptation : test formel en rapport avec les besoins, exigences et processus métier, conduit pour déterminer si un système satisfait ou non aux critères d’acceptation et permettre aux utilisateurs, clients ou autres entités autorisées de déterminer l’acceptation ou non du système [d’après IEEE 610]

##### Base de test: 
- Les besoins des utilisateurs
- Les exigences du système
- Les cas d'utilisation
- Les processus métiers
- Les rapports d'analyse de risques

##### Objets de test typique:
- Les processus métiers sur le système entièrement intégré
- Les processus opérationnels et de maintenance
- Les procédures utilisateur
- Les formulaires
- Les rapports
- Les données de configuration

Les tests d'acceptation sont souvent de la responsabilité des clients ou des utilisateurs d'un système, mais d'autres parties prenantes peuvent être impliquées également.  
L'objectif des tests d'acceptation est d'établir la confiance dans le système, les parties du système ou des caractéristiques non-fonctionnelles du système. Déceler les défauts n'est pas le principal objectif des des tests d'acceptation.  Les tests d'acceptation peuvent évaluer la préparation du système pour son déploiement et son utilisation, même si ce n'est pas nécessairement le niveau final des tests.
Par exemple, un système de test d'intégration à grande échelle peut venir après les tests d'acceptation d'un système.

Les tests d'acceptation typiques sont les suivants:

• Les tests d'acceptation utilisateur:

En règle générale vérifie l'aptitude à l'utilisation du système par les utilisateurs métier.

• Les tests d'acceptation opérationnels:

L'acceptation du système par les administrateurs système, y compris:

• Contrôle de sauvegarde / restauration

• Reprise après sinistre

• Gestion des utilisateurs

• Les tâches de maintenance

• Chargement de données et les tâches de migration

• Des contrôles périodiques des failles de sécurité

• Les tests d'acceptation contractuels et réglementaires:

Les tests d'acceptation contractuels sont effectués par rapport aux critères d'acceptation du contrat. 

Les critères d'acceptation doivent être définis par les parties prenantes du contrat.

Les tests d'acceptation réglementaires sont effectués pour vérifier le respect des règlementations, 

comme le cadre gouvernemental, juridique ou de sécurité.

### Les types de tests

### Les catégories de tests

## Autres généralités sur les tests logiciels
