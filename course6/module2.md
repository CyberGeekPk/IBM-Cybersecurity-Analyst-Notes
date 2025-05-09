# Module 2 - SQL Basics and Database Management Fundamentals
In this module, you will explore basic SQL statements. You will also learn about essential database roles and permissions, management techniques, and the importance of backing up databases. Practical application is emphasized through hands-on labs, where you will write and practice basic SQL statements on a live database and perform fundamental database operations. The module concludes with a summary of key points and highlights, reinforcing the concepts covered.

## Learning Objectives
- Identify the syntax of the SELECT statement using the WHERE clause
- Use SELECT queries to retrieve data from the database
- Query a database to retrieve data records from one or more tables based on specified criteria
- Explain how to use SQL expressions like COUNT, DISTINCT, and LIMIT in SELECT statements to manage and retrieve data
- Apply SQL techniques to retrieve specific row counts, eliminate duplicates, and restrict the number of rows retrieved from a table
- Identify the syntax of the INSERT statement and explain two methods for adding rows to a table
- Explain the syntax and importance of the UPDATE and DELETE statements and the WHERE clause
- Apply key DML SQL statements to insert, update, and delete data in tables
- Describe how database permissions work and identify the benefits of roles in a database
- Explain database management and review major SQL command categories
- List the types of database backups and their importance
- Execute SQL commands to perform basic database operations

# SQL Basics

## SELECT command
- The SELECT command is used in SQL (Structured Query Language) to retrieve data from a database.
- Basic Syntax of SELECT: SELECT column1, column2 FROM table_name;

### Important Concepts Related to SELECT:
- Selecting All Columns: If you want to get every column from a table, use * instead of specifying column names.
- SELECT * FROM employees;
- Filtering Data with WHERE: You can filter the results to get only the data you want by using the WHERE clause.
- SELECT first_name, last_name FROM employees WHERE department = 'Sales';
- Sorting Data with ORDER BY: You can sort your results using ORDER BY. By default, it sorts in ascending order, but you can specify descending order as well.
- SELECT first_name, last_name FROM employees ORDER BY last_name ASC;
- Limiting Results with LIMIT: If you only want to retrieve a certain number of rows, you can use LIMIT.
- Aggregating Data with Functions: SQL has several built-in functions to summarize or perform calculations on data. Common ones are COUNT(), SUM(), AVG(), MIN(), and MAX().
- Grouping Data with GROUP BY: When you need to group rows based on a column and apply aggregate functions like COUNT() or SUM(), you can use GROUP BY.
- Combining Data with JOIN: Sometimes, you need to get data from multiple tables. This is where JOIN comes in. A JOIN combines rows from two or more tables based on a related column between them.
- Using Aliases: You can give tables and columns temporary names (aliases) to make queries easier to read.

### COUNT
The COUNT command in SQL is used to count the number of rows that match a specific condition in a database. It is an aggregate function, which means it performs a calculation on a set of values to return a single result.

#### Basic Syntax of COUNT:
- SELECT COUNT(column_name)
- FROM table_name;

### DISTINCT
The DISTINCT command in SQL is used to remove duplicate values from the result set. It ensures that the query returns only unique values.

#### Basic Syntax of DISTINCT:
- SELECT DISTINCT column_name
- FROM table_name;

### LIMIT
The LIMIT command in SQL is used to limit the number of rows returned by a query. This is helpful when you only want to see a specific number of results, instead of the entire dataset, which might be very large.

#### Basic Syntax of LIMIT:
- SELECT column_name
- FROM table_name
- LIMIT number;

### INSERT Command
The INSERT command is used to insert data into a table. It allows you to add one or more rows of data to a specified table in your database.

#### Basic Syntax of INSERT:
- INSERT INTO table_name (column1, column2, column3, ...)
- VALUES (value1, value2, value3, ...);

### UPDATE Command
The UPDATE command is used to modify existing records in a table. You can use it to change the values of one or more columns in a particular row or set of rows.

#### Basic Syntax of UPDATE:
- UPDATE table_name
- SET column1 = value1, column2 = value2, ...
- WHERE condition;

### DELETE Command
The DELETE command is used to remove rows from a table. You can delete all rows or just a specific set of rows based on a condition.

#### Basic Syntax of DELETE:
- DELETE FROM table_name
- WHERE condition;

# Roles, Permissions & Backup

## Database Roles and Permissions
Permissions provide the authority to access a database, tables, objects, and other system resources in a specified manner to allow selection, insertion, or modification of data rows. A database role is a collection of any number of permissions that can be assigned to one or more users. Roles allow granting and managing sets of permissions for various categories of users, rather than granting those permissions to each user individually. And roles can be granted and revoked at any time, allowing for more flexibility in maintaining a database.

## Database Management
SQL commands are the instructions used to communicate with a database to perform tasks, functions, and queries with data. SQL commands can be used to search the database and perform other functions like creating tables, adding data to tables, modifying data, and dropping tables. SQL commands are grouped into three major categories depending on their functionality: DDL commands that are used for creating, modifying, and dropping the structure of database objects; DML commands that are used for storing, retrieving, modifying, and deleting data; and DCL commands that are used for providing security to database objects. And data is input into a database using the queries CREATE database, CREATE table, and INSERT INTO table, and data is extracted by using queries and reporting software tools such as ClearPoint, SAP Crystal Reports, and Jaspersoft reporting.

## Backing Up Databases 
A logical backup contains copies of information about a database and physical backups are copies of directories and data files, including data controls, transaction files, and archived logs. Backup copies allow data to be restored from an earlier point in time to help the business recover from an unplanned event. Storing the copy of the data on a separate medium is critical to protect against primary data loss or corruption. And there are four main methods of backing up a database: full, which is a copy of all files following an automatic preset schedule; differential, which includes the last full backup and the last differential backup; incremental, which saves storage by backing up the files generated or updated since the last backup; and virtual, which uses a database to track and maintain backup data.
