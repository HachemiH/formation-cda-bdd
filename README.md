# 4.2.4.8 Sélectionner les commandes dont le produit est soit une 'Table', soit un 'Bureau'.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE Produit IN ('Table', 'Bureau');
```