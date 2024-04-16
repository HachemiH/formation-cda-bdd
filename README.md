# 3.9.3.2 Correction de la Table `Restaurants` pour Respecter la 3NF

Pour appliquer la 3NF à la table `Restaurants`, il était nécessaire de séparer les informations sur la localisation des détails spécifiques aux restaurants, car la `Ville` est fonctionnellement dépendante de l'`Adresse` et non directement de l'`ID_Restaurant`, formant une dépendance transitive.

**Table `Restaurants`**

| ID_Restaurant | Nom_Restaurant | Type_Cuisine | ID_Localisation |
| ------------- | -------------- | ------------ | --------------- |
| 1             | Chez Anne      | Française    | L1              |
| 2             | Bella Napoli   | Italienne    | L2              |

**Table `Localisations`**

| ID_Localisation | Adresse         | Ville |
| --------------- | --------------- | ----- |
| L1              | 10 rue de Paris | Paris |
| L2              | 25 via Roma     | Rome  |