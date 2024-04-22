# 4.2.4.6 Sélectionner les commandes dont la quantité est supérieure à 1, triées par date de commande de manière ascendante.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE Quantité > 1 ORDER BY Date_commande ASC;
```