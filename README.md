# SQL
SQL Portfolio

CREATE TABLE store (id INTEGER PRIMARY KEY,item TEXT, quantity INTEGER, popularity INTEGER, price INTEGER);

INSERT INTO store VALUES (1,"Graphic shirts", 95,50,15.00);
INSERT INTO store VALUES (2,"Crop tops",100,67,20.00);
INSERT INTO store VALUES (3, "Sheer tops",75,49,30.00);
INSERT INTO store VALUES (4,"Jean shorts",70,75,45.00);
INSERT INTO store VALUES (5,"Jeans",50,87,75.00);
INSERT INTO store VALUES (6,"Bathing suit tops",80,100,38.00);
INSERT INTO store VALUES (7,"Bathing suit bottoms",85,98,38.00);
INSERT INTO store VALUES (8,"Bathing suit coverups ",40,50,30.00);
INSERT INTO store VALUES (9,"Sandles",58,62,35.00);
INSERT INTO store VALUES (10,"Sneakers",29,39,55.00);
INSERT INTO store VALUES (11,"Underwear",300,95,10.00);
INSERT INTO store VALUES (12,"Bras",100,45,30.00);
INSERT INTO store VALUES (13,"Headbands",200,120,13.00);
INSERT INTO store VALUES (14,"Home Decorations",500,130,100.00);
INSERT INTO store VALUES (15,"Jewlery",200,98,35.00);

--> Order the database by price 
SELECT * FROM store ORDER BY Price;

--> What are the most popular items and their prices?
SELECT item, price, popularity FROM store ORDER BY Popularity; 

--> What are the 5 most popular items and their prices?
SELECT item, price, popularity FROM store ORDER BY Popularity limit 5;

--> What is the average price of items that have been sold at least 30 times?
SELECT AVG(price) FROM store where popularity > 30;
