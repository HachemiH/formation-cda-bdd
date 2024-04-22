# 4.2.4.4 Sélectionner les commandes passées entre le 1er avril 2023 et le 30 juin 2023.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM Commandes WHERE Date_commande BETWEEN '2023-04-01' AND '2023-06-30';
```

Voici le résulat de la requête :

| Commande_id | Client_nom | Produit    | Quantité | Prix_Unitaire | Date_commande | Ville_livraison | Catégorie_produit |
| ----------- | ---------- | ---------- | -------- | ------------- | ------------- | --------------- | ----------------- |
| 1           | Léa        | Chaise     | 2        | 25            | 2023-04-12    | Paris           | Mobilier          |
| 2           | Marc       | Table      | 1        | 50            | 2023-05-15    | Lyon            | Mobilier          |
| 3           | Julie      | Lampe      | 3        | 15            | 2023-04-18    | Paris           | Éclairage         |
| 5           | Léa        | Smartphone | 1        | 300           | 2023-06-02    | Paris           | Électronique      |