# 4.2.4.4 Sélectionner les commandes passées entre le 1er avril 2023 et le 30 juin 2023.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE Date_commande BETWEEN '2023-04-01' AND '2023-06-30';
```