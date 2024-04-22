# 4.2.4.2 Sélectionner les commandes de la catégorie 'Mobilier', triées par prix unitaire de manière descendante.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE Catégorie_produit = 'Mobilier' ORDER BY Prix_Unitaire DESC;
```