# Les tests logiciels - Classifications
TODO Graphique 3 dimensions
## Les niveaux de test
Il existe plusieurs niveaux de tests :

- Les tests de composants (ou tests unitaires)
- Les tests d'intégration
- Les tests système
- Les tests d'acceptation

### Test de composant (tests unitaires)
#### Définitions
- **Composant** : un élément logiciel minimal qui peut être testé isolément.
- **Test de composant** : le test de composants logiciels individuels [d’après IEEE 610]

Les tests de composants (également connu comme tests unitaires, tests de module ou tests de programme) vérifient le fonctionnement des modules logiciels, des programmes, des objets, des classes, etc
Ils peuvent être réalisés indépendamment du reste du système.

#### Eléments servant de base de test
- les stories
- le code source
- les exigences de composants
- la conception technique détaillée

#### Exemples de test typique
- les composants (classe, méthode ...)
- les programmes
- les conversions de données
- les migrations de données

### Test d'intégration
#### Définitions
- **Intégration** : le processus de combiner des composants ou des systèmes en assemblages plus grands.
- **Tests d’intégration** : tests effectués pour montrer des défauts dans les interfaces et interactions des composants ou des systèmes intégrés.

Les tests d'Intégration testent les interfaces entre les composants, les interactions entre les différentes parties d'un système, tels que le système d'exploitation, le système de fichiers, le matériel, et les interfaces entre les systèmes.

#### Eléments servant de base de test
- les epics
- les cas d'utilisation
- les éléments d'architecture
- les workflows

#### Exemples de test typique
- les interfaces utilisateurs
- l'implémentation de sous-systèmes
- les Bundles
- l'infrastructure
- les données de configuration

### Test système
#### Définitions
- **Système** : une collection de composants organisés pour accomplir une fonction ou un ensemble de fonctions spécifiques [IEEE 610]
- **Tests système** : le processus de test d’un système intégré pour vérifier qu’il réponde à des exigences spécifiques [Hetzel]

Les tests système prennent en compte le comportement de l'intégralité d'un système. La portée des tests doit être clairement abordée dans le plan de test.  L'environnement de test doit correspondre à l'environnement de production final autant que possible afin de minimiser le risque de défaillances spécifiques à l'environnement de test.

#### Eléments servant de base de test
- les spécifications fonctionnelles
- les cas d'utilisations
- les rapports d'analyse des risques

#### Exemples de test typique

- les blocs fonctionnels
- les manuels d'utilisation, de fonctionnement et du système
- l'installation du système
- les données de configuration

### Tests d'acceptation
#### Définitions
- **Critère d’acceptation** : le critère de sortie que doit satisfaire un composant ou un système de façon à être accepté par un utilisateur, client ou une autre entité autorisée [IEEE 610]
- **Test d’acceptation** : test formel en rapport avec les besoins, exigences et processus métier, conduit pour déterminer si un système satisfait ou non aux critères d’acceptation et permettre aux utilisateurs, clients ou autres entités autorisées de déterminer l’acceptation ou non du système [IEEE 610]

#### Eléments servant de base de test
- les besoins des utilisateurs
- les exigences du système
- les cas d'utilisation
- les processus métiers
- les rapports d'analyse de risques

#### Exemples de test typique
- les processus métiers sur le système entièrement intégré
- les processus opérationnels et de maintenance
- les procédures utilisateur
- les formulaires
- les rapports
- les données de configuration

Les tests d'acceptation sont souvent de la responsabilité des clients ou des utilisateurs d'un système, mais d'autres parties prenantes peuvent également être impliquées.  
L'objectif des tests d'acceptation est d'établir la confiance dans le système, les parties du système ou des caractéristiques non-fonctionnelles du système.  
Déceler les défauts n'est pas le principal objectif des des tests d'acceptation.  Les tests d'acceptation peuvent évaluer la préparation du système pour son déploiement et son utilisation, même si ce n'est pas nécessairement le niveau final des tests.
Par exemple, un système de test d'intégration à grande échelle peut venir après les tests d'acceptation d'un système.

Les tests d'acceptation typiques sont les suivants:

- Les tests d'acceptation utilisateur:  
En règle générale vérifie l'aptitude à l'utilisation du système par les utilisateurs métier.

- Les tests d'acceptation opérationnels:  
L'acceptation du système par les administrateurs système, y compris:
  - Contrôle de sauvegarde / restauration
  - Reprise après sinistre
  - Gestion des utilisateurs
  - Les tâches de maintenance
  - Chargement de données et les tâches de migration
  - Des contrôles périodiques des failles de sécurité

- Les tests d'acceptation contractuels et réglementaires:  
Les tests d'acceptation contractuels sont effectués par rapport aux critères d'acceptation du contrat.  
Les critères d'acceptation doivent être définis par les parties prenantes du contrat.  
Les tests d'acceptation réglementaires sont effectués pour vérifier le respect des règlementations, comme le cadre gouvernemental, juridique ou de sécurité.

## Les types de tests
### Tester les fonctionnalités (Tests fonctionnels)
####Définitions
- **Fonctionnalité** : la capacité d’un produit logiciel à fournir des fonctions qui répondent à des besoins explicites ou implicites quand le logiciel est utilisé sous des conditions spécifiées [ISO 9126]
- **Test fonctionnel** : test basé sur une analyse des spécifications d’une fonctionnalité d’un composant ou système.
#### Descriptif
Les tests fonctionnels vérifient ce que l'application fait. Les tests fonctionnels peuvent être effectués à tous les niveaux de test.

Les fonctions d'un système, sous-système ou composant peuvent être décrites dans les spécifications des exigences, des cas d'utilisation, fonctionnelle, ou non documentées.  
Les tests fonctionnels considèrent le comportement externe des logiciels (tests de boîte noire).

### Tester les caractéristiques non fonctionnelles d'un logiciel (Tests non fonctionnels)

#### Définitions
- **Exigence non-fonctionnelle** : une exigence qui ne se rapporte pas aux fonctionnalités, mais à des attributs tels que la fiabilité, le rendement, l'utilisabilité, la maintenabilité et la portabilité.
- **Tests non-fonctionnels** : test des attributs d’un composant ou système qui ne sont pas liés aux fonctionnalités (p.ex. fiabilité, rendement, utilisabilité, maintenabilité et portabilité)

#### Descriptif

Les tests non-fonctionnels comprennent:

- les tests de performance
- les  tests de charge
- les tests de stress
- les tests d'utilisabilité
- les tests de maintenabilité
- les tests de fiabilité
- les tests de portabilité
- ...

Les tests fonctionnels vérifient le "comment" l'application fonctionne.

Les tests non-fonctionnels peuvent être effectués à tous les niveaux de test. Le terme non-fonctionnel décrit les tests requis pour mesurer les caractéristiques des systèmes et des logiciels qui peuvent être quantifiés sur une échelle, comme les temps de réponse pour les tests de performance. Ces tests peuvent se référer à un modèle de qualité. Les tests fonctionnels considèrent, dans la plupart des cas, le comportement externe des logiciels (tests de boîte noire).

### Tester la structure/architecture d'un logiciel (Tests structurels)
#### Définitions
- **Test structurel**: tests basés sur une analyse de la structure interne du composant ou système

### Descriptif

Les tests structurels (boîte blanche) peuvent être effectués à tous les niveaux de test. Ces tests sont plus pertinents lorsqu'ils sont réalisés après la spécification technique, afin d'aider à mesurer la rigueur des tests grâce à l'évaluation de leur couverture. Les tests structurels doivent être basés sur l'architecture du système, comme une hiérarchie d'appels par exemple. 

### Tester les changements (Tests de régression, re-tester)
#### Définitions
- Test de régression : tests d’un programme préalablement testé, après une modification, pour s’assurer que des défauts n’ont pas été introduits ou découverts dans des parties non modifiées du logiciel, comme suites des modifications effectuées. Ces tests sont effectués quand le logiciel ou son environnement est modifié.

#### Descriptifs
Après qu'un défaut soit détecté et corrigé, le logiciel doit être re-testé pour s'assurer que le défaut original a été supprimé avec succès. Cela s'appelle la confirmation. Le débogage est une activité de développement, et non une activité de test.
Les tests de régression sont la répétition des tests d'un programme déjà testé, après une modification, afin de vérifier que des défauts n'ont pas été introduits à la suite du changement. Ces défauts peuvent être dans le logiciel testé, ou dans un autre composant logiciel connexes ou non. Ces tests sont effectués lorsque le logiciel,  ou son environnement,  est modifié.  L'étendue des tests de régression est fondée sur le risque de ne pas trouver des défauts sur un logiciel qui fonctionné correctement précédemment. Les tests doivent être reproductibles.Les tests de régression peuvent être réalisés à tous les niveaux de tests, et comprend les tests fonctionnels, non fonctionnels et structurels.

## Les catégories de test

Le but d'une conception de tests est de déterminer les conditions de tests, les cas de test, et les données de test.  
La distinction classique pour désigner les techniques de conception des tests est la suivante:

- Techniques boîte noire
- Techniques boîte blanche
- Techniques basées sur l'expérience 

### Techniques boites noire

#### Définitions
- **Tests Boîte Noire** : tests, fonctionnels ou non fonctionnels, sans référence aux structures internes du composant ou du système.
- **Technique de conception de tests boîte noire** : procédure documentée pour élaborer et sélectionner des cas de tests basés sur une analyse des spécifications, soit fonctionnelles soit non-fonctionnelles, d’un composant ou système sans faire référence à ses structures internes.

#### Descriptif
Les techniques de conception de tests boîte noire (également appelée techniques de conception basées sur les spécifications) sont des façons d'identifier et de sélectionner les conditions de tests, les cas de test, et les données de test fondée sur une analyse de la documentation de base des tests.  

Ces techniques concernent à la fois les tests fonctionnels et non fonctionnels. 

Les tests boîte noire, par définition, n'utilise aucune information concernant la structure interne du composant ou du système à tester.

Il existe des caractéristiques communes aux différentes techniques de conception de tests boites noires :

- Des modèles, formels ou informels, sont utilisés pour la spécification du problème à résoudre
- Les cas de tests peuvent être dérivés de façon systématique à partir de ces modèles

Parmi les techniques de conception de tests boites noires:
- Partitionnement par équivalence
- Analyse des valeurs limites
- Tests par Table de décision
- Test d'état-transition
- Test des cas d'utilisation

### Techniques boite blanche
#### Définition
- **Test boîte blanche** : tests basés sur une analyse de la structure interne du composant ou du système
- **Technique de conception de tests boîte blanche** : procédures documentées utilisées pour élaborer et sélectionner des cas de tests basés sur une analyse de la structure interne d’un composant ou d'un système

#### Descriptif

Les techniques de conception de tests boîte blanche (également appelé techniques de conception structurelle ou techniques de conception basée sur la structure) sont basées sur une analyse de la structure de ce composant ou de ce système. 

Il existe des caractéristiques communes aux différentes techniques de conception de tests boites blanches :

- Les informations sur la façon dont le logiciel est construit sont utilisées pour définir les cas de test (par exemple, le code et les informations de conception détaillées)
- L'étendue de la couverture du logiciel peut être mesurée pour les cas de tests existants, et des cas de tests peuvent en être dérivés de façon systématique pour augmenter la couverture

Parmi les techniques de conception de tests boites blanches :
- Tests des instructions et couvertures
- Test des décisions et couverture
- Couverture de conditions
- Couverture de conditions multiples

###Technique basée sur l'expérience

Les tests boîte noire et les tests boîte blanche peuvent également s'appuyer sur l'expérience des développeurs, des testeurs et des utilisateurs afin de déterminer ce qui doit être testé. Certains tests tombent clairement dans une seule catégorie, d'autres ont des éléments des deux catégories.

Il existe des caractéristiques communes aux différentes techniques de conception de tests basées sur l'expérience:

- Les connaissances et l'expérience des personnes sont utilisées pour calculer les cas de test
- La connaissance des testeurs, des développeurs, des utilisateurs et d'autres intervenants sur le logiciel, son utilisation et son environnement est une source d'information
- La connaissance des défauts probable et leur répartition est une autre source d'information

### Choix de la technique de test

Le choix des techniques de test à utiliser dépend d'un certain nombre de facteurs, comme le type de système, les normes réglementaires, le client ou les exigences contractuelles, le niveau de risque, le type de risque, l'objectif du test, la documentation disponible, la connaissance des testeurs, le temps et le budget, le cycle de vie du développement cycle, les cas d'utilisation et de l'expérience acquise.

Certaines techniques sont plus adaptées à certaines situations et à certains niveaux de tests, d'autres sont applicables à tous les niveaux.

Lors de la création des cas de test, les testeurs utilisent généralement une combinaison des techniques.
