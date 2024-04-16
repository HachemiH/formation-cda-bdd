# 3.9.2.1 Correction de la Table `VentesProduits` pour Respecter la 2NF

Pour appliquer la 2NF à la table `VentesProduits`, il fallait séparer les informations relatives au produit des détails de la vente, car le `Nom_Produit` dépend uniquement de l'`ID_Produit` et non de la combinaison de l'`ID_Vente` et de l'`ID_Produit`.

**Table `Produits` après correction :**

| ID_Produit | Nom_Produit   |
| ---------- | ------------- |
| 100        | Café Arabica  |
| 101        | Thé Earl Grey |

**Table `Ventes` après correction :**

| ID_Vente | ID_Produit | Quantité | Date_Vente |
| -------- | ---------- | -------- | ---------- |
| 1        | 100        | 2        | 2024-04-15 |
| 2        | 101        | 1        | 2024-04-16 |
| 3        | 100        | 3        | 2024-04-17 |

Cette correction implique la création d'une table séparée pour les produits pour éliminer la dépendance partielle, assurant ainsi que chaque information soit pleinement fonctionnellement dépendante de la clé primaire, conforme à la 2NF.