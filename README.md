# 3.9.2.3 Correction de la Table `InscriptionsActivités` pour Respecter la 2NF

Pour appliquer la 2NF à la table `InscriptionsActivités`, il fallait séparer les informations personnelles des participants des détails de leur inscription, car les informations `Nom_Participant` et `Âge_Participant` dépendent uniquement de l'`ID_Participant`, et non de la combinaison de l'`ID_Activité` et de l'`ID_Participant`.

**Table `Participants` après correction :**

| ID_Participant | Nom_Participant | Âge_Participant |
| -------------- | --------------- | --------------- |
| 001            | Alice L'eau     | 12              |
| 002            | Bob Zen         | 34              |

**Table `Inscriptions` après correction :**

| ID_Activité | ID_Participant | Nom_Activité |
| ----------- | -------------- | ------------ |
| A1          | 001            | Natation     |
| B2          | 002            | Yoga         |

Cette correction implique la création de deux tables : une pour les détails des participants (`Participants`) et une autre pour leurs inscriptions aux activités (`Inscriptions`), garantissant ainsi que chaque donnée est pleinement fonctionnellement dépendante de la clé primaire complète, en conformité avec la 2NF.