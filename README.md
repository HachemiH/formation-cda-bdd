# 4.2.4.7 Sélectionner toutes les commandes de 'Marc' ou 'Julie', excluant celles livrées à 'Nantes'.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE (Client_nom = 'Marc' OR Client_nom = 'Julie') AND Ville_livraison != 'Nantes';
```

Voici le résulat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 2           | Marc       | Table   | 1        | 50            | 2023-05-15    | Lyon            | Mobilier          |
| 3           | Julie      | Lampe   | 3        | 15            | 2023-04-18    | Paris           | Éclairage         |
| 6           | Marc       | Clavier | 2        | 20            | 2023-07-19    | Lyon            | Électronique      |
| 7           | Julie      | Souris  | 1        | 10            | 2023-08-05    | Paris           | Électronique      |
| 10          | Marc       | Chaise  | 4        | 25            | 2023-11-12    | Lyon            | Mobilier          |
