# 4.2.4.3 Sélectionner toutes les commandes livrées à 'Paris' qui ne sont pas de la catégorie 'Électronique'.

Voici la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Ville_livraison = 'Paris' AND Catégorie_produit != 'Électronique';
```

Voici le résulat de la requête :

| Commande_id | Client_nom | Produit | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 1           | Léa        | Chaise  | 2        | 25            | 2023-04-12    | Paris           | Mobilier          |
| 3           | Julie      | Lampe   | 3        | 15            | 2023-04-18    | Paris           | Éclairage         |
| 9           | Léa        | Lampe   | 2        | 15            | 2023-10-03    | Paris           | Éclairage         |