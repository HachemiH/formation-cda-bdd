# 2.7.3.3 Écrire le code SQL de la table `Orders`.

```sql
CREATE TABLE public.Orders(
	order_id      SERIAL NOT NULL,
	total_price   FLOAT NOT NULL,
	customer_id   INT NOT NULL,
	CONSTRAINT Orders_PK PRIMARY KEY (order_id),
  CONSTRAINT Orders_Customers_FK FOREIGN KEY (customer_id) REFERENCES public.Customers(id)
)WITHOUT OIDS;
```

Ici, on modifie le nom du champ `id` par `customer_id` dans un soucis de clareté.