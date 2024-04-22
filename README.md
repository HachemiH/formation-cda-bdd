# 4.2.4.7 Sélectionner toutes les commandes de 'Marc' ou 'Julie', excluant celles livrées à 'Nantes'.

Voilà la requête conrrespondante pour réaliser l'opération.

```sql
SELECT * FROM commandes WHERE (Client_nom = 'Marc' OR Client_nom = 'Julie') AND Ville_livraison <> 'Nantes';
```