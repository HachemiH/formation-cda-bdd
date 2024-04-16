# 2.7.1.6 Créer une relation nommée `include`.

Voilà le résultat attendu après la création de la relation `include`.

![](./assets/solution.png)

Ici on voit que :

- Les cardinalités de la relation `include` du côté de l'entité `Products` est `0,n`.
- Les cardinalités de la relation `include` du côté de l'entité `Orders` est `1,n`.

Ce qui traduit qu'un `Product` peut n'être lié à aucune **OU** plusieurs `Orders`. Et qu'une `Order` est forcément liée à un **OU** plusieurs `Products`.