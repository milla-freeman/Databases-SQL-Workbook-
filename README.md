# 📊 Databases & SQL Project

### SQL Fundamentals • Joins • Queries • MySQL Workbench

---

## 📌 Project Overview

This project documents my SQL learning journey completed during my data analytics training.
It includes practical exercises using relational databases and covers:

* SQL fundamentals
* Filtering and sorting data
* JOINs
* Aggregations
* Real business-style scenarios
* Bonus practice exercises (SQLBolt up to Exercise 12)

All queries were written and tested in **MySQL Workbench**.

---

## 🗂️ Files Included

* **Databases & SQL Workbook.docx** – full SQL answers and explanations
* SQL scripts (if added separately)
* Screenshots of executed queries

---

## 📘 What I Learned

### ➤ SQL Foundations

* `SELECT` statements
* `WHERE` filtering
* `DISTINCT`
* `ORDER BY`
* `BETWEEN`, `IN`, `AND`/`OR`
* `LIMIT`

### ➤ Joins

* `INNER JOIN`
* `LEFT JOIN`
* `RIGHT JOIN`
* `SELF JOIN`
* `CROSS JOIN`
* Understanding of relational database structure

### ➤ Aggregation

* `COUNT()`
* `SUM()`
* `AVG()`
* `GROUP BY`
* Ordering aggregated results

---

## 🛠️ Tools Used

* **MySQL Workbench**
* Relational sample databases
* SQLBolt (Exercises 1–12)

---

## 📂 Sample Queries

### Retrieve all customers

```sql
SELECT * 
FROM Customers;
```

### Products over £50

```sql
SELECT *
FROM Products
WHERE Price > 50;
```

### Orders with customer & employee names

```sql
SELECT o.OrderID, o.OrderDate, c.CustomerName, 
       CONCAT(e.FirstName, ' ', e.LastName) AS EmployeeName
FROM Orders AS o
JOIN Customers AS c ON o.CustomerID = c.CustomerID
JOIN Employees AS e ON o.EmployeeID = e.EmployeeID;
```

### Cities in the USA

```sql
SELECT COUNT(*) 
FROM city
WHERE CountryCode = 'USA';
```

---

## 🌍 Realistic SQL Tasks Completed

### Business-style tasks included:

* Creating customer marketing lists
* Filtering products based on cost and stock
* Linking products to suppliers
* Analysing categories and sales performance
* Reviewing year-specific orders
* Summarising quantity and revenue

### Additional real-world questions covered:

* Ranking cities by population
* Filtering city names by patterns
* Identifying highest/lowest values in datasets
* Exploring country-level data

---

## 📝 Reflection

This project helped me:

* Strengthen my SQL foundations
* Understand relational database structures
* Translate business questions into SQL queries
* Use joins and aggregations to build meaningful insights
* Build confidence using MySQL Workbench

---

## 🚀 Future Improvements

* Write more complex multi-join queries
* Add stored procedures and views
* Optimise queries for performance
* Explore PostgreSQL and more advanced functions

