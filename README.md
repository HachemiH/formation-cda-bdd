# 2.7.3.3 Écrire le code SQL de la table `Orders`.

```sql
CREATE TABLE Orders(
	order_id      SERIAL NOT NULL,
	total_price   FLOAT NOT NULL,
	id            INT NOT NULL,
	CONSTRAINT Orders_PK PRIMARY KEY (order_id),
  CONSTRAINT Orders_Customers_FK FOREIGN KEY (id) REFERENCES public.Customers(id)
)WITHOUT OIDS;
```