# 2.7.3.1 Écrire le code SQL de la table `Products`.

```sql
CREATE TABLE public.Products(
	id              SERIAL NOT NULL,
	product_name    VARCHAR (50) NOT NULL,
	unitary_price   FLOAT NOT NULL,
	quantity        INT NOT NULL,
	CONSTRAINT Products_PK PRIMARY KEY (id)
)WITHOUT OIDS;
```