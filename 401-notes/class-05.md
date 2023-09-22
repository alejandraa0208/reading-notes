# Class 05 Notes

## SQL Cheat Sheet

### SQL Basics

SQL stands for Structured Query Language.

SQL is used to manage and manipulate relational databases.

### Common SQL Statements

#### SELECT: Retrieve data from a database

SELECT column1, column2

FROM table_name

WHERE condition;

#### INSERT: Insert new data into a table

INSERT INTO table_name (column1, column2)

VALUES (value1, value2);

#### UPDATE: Modify existing data in a table

UPDATE table_name

SET column1 = new_value

WHERE condition;

#### DELETE: Delete data from a table

DELETE FROM table_name

WHERE condition;

### SQL Clauses

WHERE: Filters data based on a specified condition.

ORDER BY: Sorts the result set.

GROUP BY: Groups rows with the same values into summary rows.

HAVING: Filters data after it has been grouped.

JOIN: Combines rows from two or more tables based on a related column.

DISTINCT: Returns unique values in a result set.

### SQL Functions

COUNT(): Counts the number of rows.

SUM(): Calculates the sum of values in a column.

AVG(): Calculates the average of values in a column.

MAX(): Finds the maximum value in a column.

MIN(): Finds the minimum value in a column.

### SQL Constraints

PRIMARY KEY: Uniquely identifies each record in a table.

FOREIGN KEY: Establishes a link between two tables.

NOT NULL: Ensures that a column cannot have a NULL value.

UNIQUE: Ensures that all values in a column are unique.

CHECK: Enforces a condition for values in a column.

### SQL Joins

INNER JOIN: Returns records that have matching values in both tables.

LEFT JOIN (or LEFT OUTER JOIN): Returns all records from the left table and matching records from the right table.

RIGHT JOIN (or RIGHT OUTER JOIN): Returns all records from the right table and matching records from the left table.

FULL JOIN (or FULL OUTER JOIN): Returns all records when there is a match in either the left or right table.

### SQL Tips

Always back up your data before making significant changes.

Use comments to document your SQL code.

Test complex queries on a small dataset before running them on a large one.

Keep your database schema well-organized with proper naming conventions.
