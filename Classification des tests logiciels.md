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
