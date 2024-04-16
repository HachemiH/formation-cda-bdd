# 3.9.1.3 Correction de la Table `PatientsConditions` pour Respecter la 1NF

Pour appliquer la 1NF à la table `PatientsConditions`, il fallait simplement séparer les conditions de santé listées ensemble pour certains patients en lignes distinctes, et diviser le champ composite `Nom` en 2 (`Prénom` et `Nom`) en garantissant une association unique entre un patient et chaque condition de santé.

**Table `PatientsConditions` :**

| PatientID | Prénom    | Nom       | Condition    |
| --------- | --------- | --------- | ------------ |
| 1         | Denise    | Legrand   | Diabète      |
| 1         | Denise    | Legrand   | Hypertension |
| 2         | Éric      | Calembour | Allergies    |
| 3         | Françoise | Dupont    | Asthme       |
| 3         | Françoise | Dupont    | Allergies    |