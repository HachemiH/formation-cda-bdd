# 4.2.4.3 Sélectionner toutes les commandes livrées à 'Paris' qui ne sont pas de la catégorie 'Électronique'.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE Ville_livraison = 'Paris' AND Catégorie_produit != 'Électronique';
```