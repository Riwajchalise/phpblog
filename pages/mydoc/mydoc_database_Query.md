---
title: Database query
keywords: database_query,database
last_updated: December 16, 2019
tags: 
summary: "This post discusses basic SQL Query used in this lesson."
sidebar: mydoc_sidebar
permalink: mydoc_database_Query.html
folder: mydoc
---

A database query is a request for data from a database. The request is to retrive and manipulate data from the database.

## Select
Select statement is used to select data from database. It returns the stored data from the database.

### Syntax
```
SELECT column1, column2, ...
FROM table_name;
```
To select all field available in the table we use * insted of column name.

```
SELECT * FROM table_name;
```

## Insert into
The insert into statement is used to insert new record in the table.

### Syntax

```
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

## Update
The Update statement is used to modify the existing record in the table.

### Syntax

```
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```
### Example

```
UPDATE Customers
SET ContactName = 'Somthing', City= 'iland'
WHERE CustomerID = 1;
```

## Delete
The delete statement is used to delete existing record in the table.

### Syntax
```
DELETE FROM table_name WHERE condition;
```

### Example

```
DELETE FROM Customers WHERE CustomerName='something';
```