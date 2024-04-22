# 4.2.4.2 Sélectionner les commandes de la catégorie 'Mobilier', triées par prix unitaire de manière descendante.

Voici la requête correspondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Catégorie_produit = 'Mobilier' ORDER BY Prix_Unitaire DESC;
```

Voici le résultat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 4           | Luc        | Bureau  | 1        | 100           | 2023-03-22    | Nantes          | Mobilier          |
| 2           | Marc       | Table   | 1        | 50            | 2023-05-15    | Lyon            | Mobilier          |
| 1           | Léa        | Chaise  | 2        | 25            | 2023-04-12    | Paris           | Mobilier          |
| 10          | Marc       | Chaise  | 4        | 25            | 2023-11-12    | Lyon            | Mobilier          |