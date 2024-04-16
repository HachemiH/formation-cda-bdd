# 3.9.1.3 Correction de la Table `PatientsConditions` pour Respecter la 1NF

Pour appliquer la 1NF à la table `PatientsConditions`, il fallait simplement séparer les conditions de santé listées ensemble pour certains patients en lignes distinctes, garantissant une association unique entre un patient et chaque condition de santé.

**Table `PatientsConditions` :**

| PatientID | Nom       | Condition    |
| --------- | --------- | ------------ |
| 1         | Denise    | Diabète      |
| 1         | Denise    | Hypertension |
| 2         | Éric      | Allergies    |
| 3         | Françoise | Asthme       |
| 3         | Françoise | Allergies    |