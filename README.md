# 3.9.3.3 Correction de la Table `Cours` pour Respecter la 3NF

Pour aligner la table `Cours` avec la 3NF, il était essentiel de retirer la dépendance transitive en créant une table distincte pour les professeurs, car `Département_Professeur` est dépendant de `Professeur`, et non directement de `ID_Cours`.

**Table `Cours` :**

| ID_Cours | Titre_Cours   | ID_Professeur |
| -------- | ------------- | ------------- |
| C101     | Mathématiques | P1            |
| C102     | Informatique  | P2            |

**Table `Professeurs` :**

| ID_Professeur | Nom_Professeur | Département_Professeur |
| ------------- | -------------- | ---------------------- |
| P1            | Mme. Durant    | Mathématiques          |
| P2            | M. Dupont      | Informatique           |

Cette structuration sépare les informations sur les cours des détails spécifiques aux professeurs, éliminant ainsi la dépendance transitive pour s'assurer que toutes les données de chaque table sont directement dépendantes de leurs clés primaires.