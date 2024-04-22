# 4.2.4.5 Sélectionner les noms des clients et les produits commandés, pour les commandes contenant des produits dont le nom commence par 'C'.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT Client_nom, Produit FROM commandes WHERE Produit LIKE 'C%';
```