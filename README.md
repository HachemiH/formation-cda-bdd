# 4.2.4.6 Sélectionner les commandes dont la quantité est supérieure à 1, triées par date de commande de manière ascendante.

Voici la requête correspondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Quantité > 1 ORDER BY Date_commande ASC;
```

Voici le résulat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 1           | Léa        | Chaise  | 2        | 25            | 2023-04-12    | Paris           | Mobilier          |
| 3           | Julie      | Lampe   | 3        | 15            | 2023-04-18    | Paris           | Éclairage         |
| 6           | Marc       | Clavier | 2        | 20            | 2023-07-19    | Lyon            | Électronique      |
| 9           | Léa        | Lampe   | 2        | 15            | 2023-10-03    | Paris           | Éclairage         |
| 10          | Marc       | Chaise  | 4        | 25            | 2023-11-12    | Lyon            | Mobilier          |
