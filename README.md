# 2.7.1.7 Écrire le dictionnaire de données.

Voici le dictionnaire de données à produire pour cette application :

| Nom de l'attribut  | Type de donnée       | Contrainte | Taille | Exemple                                                                    |
| ------------------ | -------------------- | ---------- | ------ | -------------------------------------------------------------------------- |
| id                 | Auto_Increment (INT) | PK         | N/A    | 0, 1, ...                                                                  |
| product_name       | VARCHAR              | N/A        | 50     | Vélo, Aspirateur, ...                                                      |
| unitary_price      | FLOAT                | N/A        | N/A    | 59.99, 21.99, ...                                                          |
| quantity           | INT                  | N/A        | N/A    | 1, 2, ...                                                                  |
| order_id           | Auto_Increment (INT) | PK         | N/A    | 0, 1, ...                                                                  |
| total_price        | FLOAT                | N/A        | N/A    | 99.99, 19.99                                                               |
| customer_lastname  | VARCHAR              | N/A        | 20     | Dupont, Legrand                                                            |
| customer_firstname | VARCHAR              | N/A        | 20     | Emma, Jonathan                                                             |
| customer_mail      | VARCHAR              | N/A        | 60     | emma.dupont@laposte.net, jonathan.legrand@outlook.fr                       |
| customer_address   | VARCHAR              | N/A        | 60     | 3 Rue de la Boustify, 76310, Le Havre, 4 Rue de la Boustify, 49000, Angers |