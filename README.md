SELECT is used to select data from a table in a database. Example: SELECT * FROM Customers
SELECT DISTINCT is used to select only unique values from a table. Example: SELECT DISTINCT Country FROM Customers
WHERE is used to filter rows in a query based on a specified condition. Example: SELECT * FROM Customers WHERE City = 'London'
ORDER BY is used to sort the result set of a query in ascending or descending order. Example: SELECT * FROM Customers ORDER BY Country DESC
AND operator is used to combine multiple conditions in a WHERE clause. Example: SELECT * FROM Customers WHERE City = 'London' AND Country = 'UK'
OR operator is used to combine multiple conditions in a WHERE clause and returns true if any of the conditions is true. Example: SELECT * FROM Customers WHERE City = 'London' OR Country = 'UK'
Comparison operators (such as =, >, <, >=, <=, <>) are used to compare values in a query. Example: SELECT * FROM Customers WHERE Age > 30
BETWEEN is used to filter rows based on a range of values. Example: SELECT * FROM Customers WHERE Salary BETWEEN 50000 AND 80000
TOP is used to limit the number of rows returned in a query. Example: SELECT TOP 10 * FROM Customers
Aggregate functions (such as SUM(), AVG(), COUNT(), MIN(), MAX()) are used to perform calculations on a set of rows and return a single value. Example: SELECT SUM(Salary) FROM Employees
GROUP BY is used to group rows in a query based on one or more columns. Example: SELECT COUNT(*) FROM Customers GROUP BY City
HAVING is used to filter groups in a query based on a specified condition. Example: SELECT COUNT(*) FROM Customers GROUP BY City HAVING COUNT(*) > 10
Joins are used to combine rows from two or more tables based on a related column between them.
INNER JOIN returns only matching rows from both tables. Example: SELECT * FROM Customers INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID
OUTER JOIN returns matching rows from one table and non-matching rows from another table.
LEFT JOIN returns all rows from the left table and matching rows from the right table. Example: SELECT * FROM Customers LEFT JOIN Orders ON Customers.CustomerID = Orders.CustomerID
RIGHT JOIN returns all rows from the right table and matching rows from the left table.
CROSS JOIN returns the Cartesian product of the two tables, i.e, it returns all possible combinations of rows from the two tables.
CASE WHEN is used to create a new column with a value depending on the values of other columns or expressions. Example: SELECT CustomerName, City, CASE WHEN City = 'London' THEN 'UK' ELSE 'Non-UK' END AS Country FROM Customers
Window functions (such as RANK(), DENSE_RANK(), ROW_NUMBER(), LEAD(), LAG()) are used to perform calculations

