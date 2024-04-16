# 2.7.2.1 Transformer le MCD en MLD.

![](./assets/solution.png)

Dans ce MLD, on voit que :

- La relation `include` (`many-to-many`) est devenue une table d'association
  - Elle contient 2 clés primaires (`order_id` et `id`. Ici `id` correspond à `id` de l'entité `Products`).
- La table `Orders` contient une nouvelle clé étrangère `id` qui correspond à `id` de l'entité `Customers`.
- Les types de données sont affichés pour chaques entités.