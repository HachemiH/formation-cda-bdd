# Correction de la Table `CommandesClients` pour Respecter la 2NF

Pour appliquer la 2NF à la table `CommandesClients`, il fallait dissocier les informations du client des détails de la commande, car le nom et l'adresse du client dépendent uniquement de l'ID_Client, et non de la combinaison de l'ID_Commande et de l'ID_Client.

**Table `Clients` après correction :**

| ID_Client | Nom_Client   | Adresse_Client        |
| --------- | ------------ | --------------------- |
| 456       | Jeanne Voila | 123 Rue de Paris      |
| 789       | Pierre Paul  | 456 Avenue des Fleurs |

**Table `Commandes` après correction :**

| ID_Commande | ID_Client | Date_Commande |
| ----------- | --------- | ------------- |
| 1           | 456       | 2024-04-15    |
| 2           | 789       | 2024-04-16    |

Cette restructuration a divisé les données en deux tables distinctes pour respecter la 2NF, en assurant que chaque information soit pleinement fonctionnellement dépendante de la clé primaire, améliorant ainsi l'intégrité et la gestion des données.