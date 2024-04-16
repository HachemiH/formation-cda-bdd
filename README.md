# 2.7.3.3 Écrire le code SQL de la table d'association `include`.

```sql
CREATE TABLE public.include(
	order_id   INT NOT NULL,
	product_id INT NOT NULL,
	CONSTRAINT include_PK PRIMARY KEY (order_id, product_id),
  CONSTRAINT include_Orders_FK FOREIGN KEY (order_id) REFERENCES public.Orders(order_id),
  CONSTRAINT include_Products0_FK FOREIGN KEY (product_id) REFERENCES public.Products(id)
)WITHOUT OIDS;
```

Ici, on modifie le champ `id` par `product_id` dans un soucis de claretè.