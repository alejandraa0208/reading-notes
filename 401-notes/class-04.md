# Class 04

## Reading

### nosql vs sql

What type of database is the best fit for the complex query intensive environment?

- SQL is best fit due ensuring data consistency.

What type of database is the best fit for hierarchical data storage?

- NoSQL database like document-based like MongoDB.

Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

- SQL are like traditional libraries that are organized. NoSQL are like digital libraries where you can add more without worry about physical shelves - its easy to expand.

### sql modeling techniques

Among data tables, what is a one-to-many relationship and how do we “relate” them?

- A one-to-many relationship is a type of association between two tables where one record in the first table can be related to multiple records in the second.

We relate them by using primary and foreign keys.

Prior to designing your relational database, it might be useful to create an Entity-Relationship Diagram of the database tables and their relationships.

Explain the difference between a primary and foreign key.

- Different between is primary key is a colum in a database and uniquely identifies each record in that table. A foreign key is a column in one table that refers to the primary key and establishes a relationship between tables by linking records.

## Videos

### sql vs nosql

How do we treat keywords and parameters differently in SQL syntax?

- Keywords are reversed words in SQL that have specific meanings and functions.

Parameters are values that are used as placeholders in SQL statements.

Define normalization within the context of schemas and data.

- Is a database design process that involves organizing ddata in a relational database to reduce redundancy and dependency when ensuring data integrity.

Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

- One-to-one relationship: Imagine you have a set of employees, and each employee has one and only one desk assigned to them. This is like a one-to-one relationship. Each employee (one side) corresponds to exactly one desk (the other side).

One-to-many relationship:Now, think about a company with departments and employees. Each department (one side) can have many employees (the other side), but each employee belongs to only one department. It's like a manager supervising multiple employees. So, it's one-to-many.

Many-to-many relationship: Suppose you have a situation where students can enroll in multiple courses, and each course can have multiple students. This is like a many-to-many relationship because there's no limit to how many students can be in a course, and a student can be in multiple courses simultaneously.
