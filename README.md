# 2.7.3.2 Écrire le code SQL de la table `Customers`.

```sql
CREATE TABLE Customers(
	id                   SERIAL NOT NULL,
	customer_lastname    VARCHAR (20) NOT NULL,
	customer_firstname   VARCHAR (20) NOT NULL,
	customer_mail        VARCHAR (60) NOT NULL,
	customer_address     VARCHAR (60) NOT NULL,
	CONSTRAINT Customers_PK PRIMARY KEY (id)
)WITHOUT OIDS;
```