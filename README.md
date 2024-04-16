# 3.9.1.2 Correction de la Table `CoursMatériaux` pour Respecter la 1NF

Pour appliquer la 1NF à la table `CoursMatériaux`, il fallait simplement décomposer la colonne `Matériaux` contenant des listes de matériaux pour chaque cours en lignes distinctes, permettant ainsi une association unique entre un cours et chaque matériel requis.

**Table `CoursMatériaux` :**

| CoursID | Nom du Cours | Matériel           |
| ------- | ------------ | ------------------ |
| 1       | Math 101     | Livre de texte     |
| 1       | Math 101     | Cahier d'exercices |
| 2       | Histoire 202 | Livre de texte     |
| 2       | Histoire 202 | Atlas              |

Cette approche a transformé les valeurs multi-valuées en valeurs atomiques et chaque matériel requis par un cours est désormais représenté par une ligne distincte, alignant la structure de la table avec les principes de la 1NF. De plus, la colonne `Matériaux` est renommée en `Matériel`.