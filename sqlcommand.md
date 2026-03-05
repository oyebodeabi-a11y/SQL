
## "SELECT QUERIES"
# To display all entries in a Customers table 
SELECT *
FROM Customers
# To display top 10 customers in a table
SELECT TOP 10 *
FROM customers;
# To display all entries in a customers table for a country
SELECT TOP 10 *
FROM customers
WHERE country IN 'Germany'
# To display all entries in a customers table for 2 countries
SELECT TOP 10 *
FROM customers
WHERE country IN ('Germany', 'Mexico');
# To display all entries in a customers table not in 2 countries
SELECT *
FROM Customers
WHERE Country NOT IN ('Mexico','Germany');
# To display customers in customers table in ascending order
SELECT *
FROM Customers
ORDER BY CustomerName ASC;
# To display customers in customers table in ascending order and country in ascending order
SELECT *
FROM Customers
ORDER BY Country ASC, CustomerName ASC;
# To display customers not in Argentina
SELECT CustomerName,City,Country FROM Customers
WHERE Country NOT IN ('Argentina');
# To display between prices
SELECT TOP 5 * FROM Products
Where Price between 18.00 and 22.00
# To show columns in Product table and arrange price in ascending order
SELECT ProductName, Price FROM Products
ORDER BY Price ASC;