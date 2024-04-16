# Correction de la Table `CoursUniversitaires` pour Respecter la 2NF

Pour appliquer la 2NF à la table `CoursUniversitaires`, il fallait éliminer la dépendance partielle en séparant les informations de l'enseignant dans une nouvelle table, car l'enseignant est uniquement dépendant de l'ID du cours et non de la combinaison de l'ID du cours et du département.

**Table `Cours` après correction :**

| ID_Cours | Département   | Nom_Cours     |
| -------- | ------------- | ------------- |
| 101      | Informatique  | Programmation |
| 102      | Mathématiques | Algèbre       |

**Table `EnseignantsCours` après correction :**

| ID_Cours | Enseignant  |
| -------- | ----------- |
| 101      | M. Dupont   |
| 102      | Mme. Durand |

La correction a impliqué la création de deux tables séparées pour respecter la 2NF : une pour les cours (`Cours`) (sans dépendance partielle) et une pour associer chaque cours à son enseignant (`EnseignantsCours`), garantissant que toutes les informations dépendent pleinement de la clé primaire.