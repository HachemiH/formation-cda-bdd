# 3.9.1 Correction de la Table `EmployésLangues` pour Respecter la 1NF

Pour appliquer la 1NF à la table `EmployésLangues`, il fallait simplement séparer les valeurs multi-valuées de la colonne `Langue` en lignes distinctes, en associant chaque employé à chaque langue parlée.

**Table `EmployésLangues` :**

| EmployéID | Nom     | Langue   |
| --------- | ------- | -------- |
| 1         | Alice   | Anglais  |
| 1         | Alice   | Français |
| 2         | Bob     | Espagnol |
| 3         | Charlie | Anglais  |
| 3         | Charlie | Allemand |

Cette modification a permis d'éliminer les valeurs multi-valuées, en s'assurant que chaque ligne contienne des informations atomiques conformes aux exigences de la 1NF.