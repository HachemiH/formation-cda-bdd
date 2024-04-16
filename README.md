# 2.7.1.5 Créer une relation nommée `is passed by`.

Voilà le résultat attendu après la création de la relation `is passed by`.

![](./assets/solution.png)

Ici on voit que :

- Les cardinalités de la relation `is passed by` du côté de l'entité `Customers` est `0,n`.
- Les cardinalités de la relation `is passed by` du côté de l'entité `Orders` est `1,1`.

Ce qui traduit qu'un `Customer` peut ne passer aucune **OU** plusieurs commandes. Et qu'une `Order` n'est passée que par un **ET** un seul `Customer`.