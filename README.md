# 3.9.3.1 Correction de la Table `Employés` pour Respecter la 3NF

Pour appliquer la 3NF à la table `Employés`, il fallait dissocier les informations du département des détails des employés, car `Nom_Département` et `Adresse_Département` sont fonctionnellement dépendants de `ID_Département`, constituant une dépendance transitive par rapport à `ID_Employé`.

**Table `Employés` après correction :**

| ID_Employé | Nom_Employé | ID_Département |
| ---------- | ----------- | -------------- |
| 1          | Alice       | D1             |
| 2          | Bob         | D2             |

**Table `Départements` après correction :**

| ID_Département | Nom_Département | Adresse_Département       |
| -------------- | --------------- | ------------------------- |
| D1             | RH              | 123 Rue des Ressources    |
| D2             | IT              | 456 Rue de l'Informatique |

Cette restructuration a impliqué la création d'une table séparée `Départements` pour éliminer la dépendance transitive, assurant ainsi que chaque information soit directement dépendante de la clé primaire de sa table respective, conforme à la 3NF.