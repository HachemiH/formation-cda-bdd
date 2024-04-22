# 4.2.4.5 Sélectionner les commandes contenant des produits dont le nom commence par 'C'.

Voici la requête correspondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Produit LIKE 'C%';
```

Voici le résulat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 1           | Léa        | Chaise  | 2        | 25            | 2023-04-12    | Paris           | Mobilier          |
| 6           | Marc       | Clavier | 2        | 20            | 2023-07-19    | Lyon            | Électronique      |
| 10          | Marc       | Chaise  | 4        | 25            | 2023-11-12    | Lyon            | Mobilier          |