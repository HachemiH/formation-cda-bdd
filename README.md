# 4.2.4.8 Sélectionner les commandes dont le produit est soit une 'Table', soit un 'Bureau'.

Voici la requête correspondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Produit IN ('Table', 'Bureau');
```

Voici le résultat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 2           | Marc       | Table   | 1        | 50            | 2023-05-15    | Lyon            | Mobilier          |
| 4           | Luc        | Bureau  | 1        | 100           | 2023-03-22    | Nantes          | Mobilier          |