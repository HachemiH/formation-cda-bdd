# 4.2.4.1 Sélectionner toutes les commandes avec un prix unitaire supérieur à 20 €

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Prix_Unitaire > 20;
```

Voici le résultat de la requête :

| Commande_id | Client_nom | Produit    | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ---------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 2           | Marc       | Table      | 1        | 50            | 2023-05-15    | Lyon            | Mobilier          |
| 4           | Luc        | Bureau     | 1        | 100           | 2023-03-22    | Nantes          | Mobilier          |
| 5           | Léa        | Smartphone | 1        | 300           | 2023-06-02    | Paris           | Électronique      |
| 8           | Luc        | Tablette   | 1        | 200           | 2023-09-15    | Nantes          | Électronique      |
| 10          | Marc       | Chaise     | 4        | 25            | 2023-11-12    | Lyon            | Mobilier          |