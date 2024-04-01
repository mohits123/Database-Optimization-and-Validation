# Database-Optimization-and-Validation
# Test Assignment: Database Optimization and Validation
##Instructions
This test assignment is designed to assess your knowledge and skills related to
database optimization and validation. Please follow the instructions carefully
and provide clear and concise answers. You may use any programming language
or tool of your choice for the coding tasks.
mysql -h 18.212.98.121 -u farhan -p classicmodels Password- farhan.

## Database Optimization

### Task 1: Caching in Database Optimization

Caching plays a crucial role in database optimization by storing frequently accessed data in memory, reducing the need for repeated disk reads. It improves query performance by fetching data from cache memory instead of the disk, resulting in faster response times. Common caching strategies include:

- Query caching: Stores the results of frequently executed queries.
- Data caching: Stores frequently accessed data in memory.
- Object caching: Caches entire objects or data structures.

### Task 2: Intelligent Archiving of Unused Tables

Intelligent archiving involves identifying and archiving unused tables in a relational database to improve performance and storage efficiency. Criteria for deciding which tables to archive may include:

- Frequency of access
- Size of the table
- Date of last access
- Business relevance

The archiving process can be implemented by:

- Moving unused tables to a separate archival database.
- Implementing a scheduled archival process based on defined criteria.

### Task 3: Role of Data Types in Database Optimization

Data types play a significant role in database optimization by optimizing storage space and improving data integrity. Examples of leveraging data types:

- Using INTEGER for primary keys and numeric data for efficient storage and indexing.
- Using VARCHAR with appropriate lengths for variable-length string data to conserve space.
- Using DATE for date values to ensure uniform formatting and efficient date-based operations.

### Task 4: Referential Integrity in Relational Databases

Referential integrity ensures that relationships between tables are maintained, contributing to data quality and consistency. It prevents orphaned or dangling records and enforces constraints on foreign key relationships. Referential integrity checks can be performed using database constraints such as FOREIGN KEY constraints and triggers.

## Data Validation

### Task 5: Primary Key Constraint

The primary key constraint ensures data quality by enforcing uniqueness and non-null entries in a table. For example, in a "Users" table, the "UserID" column can be designated as the primary key to ensure each user has a unique identifier and cannot be null.

### Task 6: Foreign Keys in Maintaining Referential Integrity

Foreign keys establish relationships between tables, maintaining referential integrity. For instance, in a "Orders" table, the "CustomerID" column can be a foreign key referencing the "UserID" column in the "Users" table, ensuring that orders are associated with existing customers.

### Task 7: CHECK Constraint in Data Validation

The CHECK constraint ensures that column values meet specified conditions. For instance, in a "Product" table, a CHECK constraint can be used to validate that the "Price" column is greater than zero.

### Task 8: Unique Constraint

The Unique constraint ensures the uniqueness of values in a column, preventing duplicate entries. For example, in a "Students" table, the "StudentID" column can be designated as unique to ensure each student has a unique identifier.

### Task 9: NOT NULL Constraint

The NOT NULL constraint ensures that a column cannot contain null values, maintaining data integrity. It should be applied to columns where null values are not acceptable, such as a "Username" column in a "Users" table.

## Coding Challenge

### Task 10: Boundary Check Python Script

Develop a Python script that performs boundary checks on a given column of data. The script should take a column name, minimum value, and maximum value as input and flag any rows in the database where the column value is outside the specified bounds.

### Task 11: Email Validation Python Function

Write a Python function that validates email addresses in a database table using regular expressions. The function should identify and flag any invalid email addresses in the specified column.

### Task 12: Automated Audits Python Script

Create a Python script that automates regular audits on a sample database. The script should connect to the database, validate entries against predefined business rules, and generate a report summarizing the results.

### Task 13: Query Log Analysis Python Script

Create a Python script that checks historical logs from the DB and predicts the most repeatable queries.

For hints and references, visit [Stack Overflow](https://stackoverflow.com/questions/650238/howto-show-the-last-queries-executed-on-mysql).


