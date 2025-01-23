## What is a Database?

- A **database** is a collection of tables.
  - Each table organizes data into **rows** (records) and **columns** (fields).
  - Databases are used to store, manage, and retrieve structured data efficiently.

### Key Concepts in a Database:

1. **Table**:

   - A table is a collection of related data entries, represented in rows and columns.
   - Example:

     | ID  | Name     | Age | City          |
     | --- | -------- | --- | ------------- |
     | 1   | John Doe | 30  | New York      |
     | 2   | Jane Doe | 25  | San Francisco |

2. **Row**:

   - A single record in a table.
   - Example: `1, John Doe, 30, New York`.

3. **Column**:

   - A field in a table, representing one attribute of the data.
   - Example: `Name` or `Age`.

4. **Primary Key**:

   - A unique identifier for each row in a table (e.g., `ID` in the above table).

5. **Foreign Key**:
   - A field in one table that links to the primary key in another table.

---

## SQL (Structured Query Language)

- **SQL** is the language used to interact with databases.
- It is used for:
  - **Creating tables** and databases.
  - **Inserting, updating, deleting, and querying data.**

## Benefits of Using Databases:

1. **Data Organization**: Stores data in a structured format.
2. **Data Integrity**: Ensures data accuracy and consistency.
3. **Efficiency**: Enables fast retrieval and management of data.
4. **Scalability**: Handles large amounts of data effectively.

## Relational Database

- defines relationship between tables of data in a relational database

## Aliasing

1. **Aliasing** helps to rename the column names for clarity

```sql
-aliasing
SELECT name AS first_name, year_hired FROM Employees;
```

2. **Aliasing** only works to the result of this particular queries

## VIEWS

- **View** refers to the table that saved the SELECT statement in virtual table
- **View** refers to the virtual table which means views are not stored in the table
-

```sql
CREATE VIEW employee_hire_years AS SELECT id,name,year_hired FROM Employees
```
