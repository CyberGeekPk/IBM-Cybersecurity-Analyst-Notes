# Module 1 : Database Fundamentals

In this module, you will be introduced to a foundational overview of data and databases, setting the stage for more advanced topics. You will begin with a course introduction outlining the key objectives and structure. You will then explore various types of data, their sources, and their uses, gaining a comprehensive understanding of both relational and non-relational databases. In addition, you’ll learn about core database fundamentals and relational data concepts. Practical application is emphasized through a hands-on lab, where you will engage with relational data concepts. You will conclude the module with a summary of key points and highlights, reinforcing the foundational knowledge necessary for progressing to more advanced database management and security topics.

## Learning Objectives
- Explain the significance of data and databases, compare relational and non-relational databases, and identify their respective uses
- Analyze the structure and relationships of relational databases to evaluate their effectiveness in managing and querying structured data
- Describe the different types of NoSQL databases and their applications to evaluate their suitability for various data storage needs
- Review the relational model, including entity-to-table mapping, data types, and the role of primary keys
- Apply your knowledge of relational database concepts and entity-relationship (ER) diagrams and analyze terms like entity, attribute, and keys

## Relational Database
A Relational Database is a way to store and organize data in tables. Each table looks like a grid (like a spreadsheet) with rows and columns.
- Rows = individual records (e.g., one student)
- Columns = fields or attributes (e.g., name, age, grade)
- The term "relational" means these tables are linked (related) to each other using keys.

### Key Concepts:
- Tables: These are like spreadsheets that hold data about one type of thing (e.g., Customers, Orders, Products)
- Rows: Each row is a single record (like one customer's information)
- Columns: These are the categories of information (like "Name", "Address", "Phone Number")
- Primary Key: A unique ID for each row (like a customer ID number)
- Foreign Key: A reference that links one table to another (like putting a customer ID in an order record)

### Important Related Concepts:
- SQL: The language used to talk to relational databases ("Structured Query Language")
- Indexes: Like a book index - helps the database find information faster
- Normalization: Organizing data to reduce duplication (makes databases more efficient)
- Transactions: Groups of operations that must all succeed or fail together (like bank transfers)
- ACID Properties: Rules that keep database operations reliable (Atomic, Consistent, Isolated, Durable)

## Non-Relational Database
A Non-Relational Database (also called NoSQL) stores data in a way other than tables. It’s flexible and better for handling large or unstructured data (like photos, videos, or big documents).
- Unlike relational databases, it doesn't need fixed table columns or strict rules.
- It’s great for apps that grow quickly or have changing data.

## Main Types of Non-Relational Databases:
### Document Stores:

- Stores data like "documents" (usually JSON format)
- Example: Customer records with all their info in one document
- Databases: MongoDB, CouchDB

### Key-Value Stores:

- Super simple: like a dictionary with keys and values
- Example: Username (key) and User Preferences (value)
- Databases: Redis, DynamoDB

### Wide-Column Stores:

- Like tables but columns can vary by row
- Good for huge datasets (billions of rows)
- Databases: Cassandra, HBase

### Graph Databases:

- Stores how things are connected (like social networks)
- Example: Who is friends with whom
- Databases: Neo4j, ArangoDB

## Relational Data Concepts
Key advantage of the relational model is logical and physical data independence and storage independence. Entities are independent objects which can have multiple characteristics called attributes. When mapping to a relational database, entities are represented as tables and attributes map to columns. Common data types include characters such as CHAR and VARCHAR, numbers such as integer and decimal, and timestamps including date and time. A primary key uniquely identifies a specific row in a table and prevents duplication of data.

## Summary: Database Fundamentals

- Databases play a crucial role in efficiently storing, managing, and querying business-critical data.
- The relational databases use structured tables and SQL, and non-relational (NoSQL) databases offer flexibility and scalability for various data types.
- Relational databases provide benefits such as data integrity, reduced redundancy, and strong backup options, though they face challenges with unstructured data and scalability in large data contexts.
- NoSQL databases offer flexible schemas and support high-scale, high-performance applications through various data models, such as key-value, document, column, and graph-based storage. However, they lack the ACID compliance and structure of relational databases.

