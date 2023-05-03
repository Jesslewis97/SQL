# SQL
SQL Portfolio

CREATE TABLE store (id INTEGER PRIMARY KEY,item TEXT, quantity INTEGER, aisle INTEGER, price INTEGER);

INSERT INTO store VALUES (1,"Shirts", 2, 1,15);
INSERT INTO store VALUES (2,"Pants",3,1,20);
INSERT INTO store VALUES (3, "Shoes",2,2,30);
INSERT INTO store VALUES (4,"Makeup", 4,3,25);
INSERT INTO store VALUES (5,"Perfume", 5,3,20);

--> How many items total are in the store, group those by the aisle they are in:
SELECT SUM(quantity) FROM store GROUP BY aisle;

--> Display the database ordered by price:
SELECT * FROM store ORDER BY price;

-> Select all items from the store that have more than 2 items: 
SELECT * FROM store WHERE quantity >2;

