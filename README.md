Ce projet repose sur un système de gestion de compte et de maintenance des états financiers. L'objectif du système de gestion comptable est de conserver un enregistrement des fonds reçus, utilisés, diffusés et donnés par une organisation. Les détails des transactions, la maintenance d'un budget et le rapprochement du solde/inventaire actuel en espèces/espèces sont incorporés dans ce système.

Le système nécessite que l'utilisateur ait les identifiants appropriés, c'est-à-dire des droits d'administrateur ou de comptable. En fonction de l'autorité d'accès, un menu d'actions possibles est affiché, et chaque option mène à une fonction qui effectue les opérations souhaitées sur des fichiers binaires grâce à l'utilisation d'objets de classe pertinents.

Les caractéristiques et fonctionnalités du système sont les suivantes :

- Interface de connexion (se divise en niveaux d'accès administrateur et comptable)
- Niveau d'accès en tant qu'administrateur ou superutilisateur
- Niveau d'accès en tant qu'un des 10 comptables prédéfinis

- Panneau/Menu de l'administrateur :
  - Saisir les détails du compte initial
  - Saisir l'historique des transactions
  - Afficher l'historique des transactions - État détaillé du compte
  - Valider les transactions actuelles pour le budget, les dépenses et les revenus
  - Afficher le budget, les revenus et les dépenses uniquement
  - Modifier les détails de la transaction
  - Afficher les détails des comptables
  - Quitter l'application

- Panneau/Menu du comptable :
  - Afficher l'historique des transactions - État détaillé du compte
  - Afficher le budget, les revenus et les dépenses uniquement
  - Afficher les détails des comptables
  - Quitter l'application

## À propos de la mise en œuvre du programme

Le système a été mis en œuvre à l'aide de diverses structures de programmation et méthodes. Il suit le concept de la programmation orientée objet en utilisant des classes et des objets pour créer une classe définissant les propriétés des transactions. Le concept de manipulation de fichiers à l'aide de fichiers binaires est incorporé pour créer et maintenir un enregistrement des transactions. Des commentaires sont présents dans l'ensemble du programme pour indiquer les fonctions et besoins de chaque composant du système.

Le programme comprend deux structures, ACCOUNT et ITEM, et une classe TRANSACTION. La structure ACCOUNT est utilisée pour représenter les informations d'identification de connexion d'un comptable individuel, c'est-à-dire le nom d'utilisateur et le mot de passe. La structure ITEM représente les détails de toute marchandise/produit acheté ou vendu par l'entreprise. La classe TRANSACTION est utilisée pour représenter les détails de chaque transaction financière de l'entreprise et pour effectuer des opérations sur cette transaction. Toutes les transactions sont stockées dans un fichier binaire, CMPNYACC.DAT, sous forme d'objets de la classe qui sont ajoutés pour conserver les enregistrements des transactions précédentes. Les fonds initiaux et les dépenses de l'entreprise sont stockés dans un autre fichier binaire, ACCDET.DAT, pour les vérifications croisées et le maintien d'un enregistrement du solde du compte.