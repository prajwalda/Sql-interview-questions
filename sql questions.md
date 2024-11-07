### 1. **Schema in SQL Server**
   - A logical grouping of tables, views, and other objects.
   - Helps organize and secure data.
   - Think of it as a “container” within the database.

### 2. **Constraints**
   - Rules applied to columns to ensure data integrity.
   - Common types: `NOT NULL`, `UNIQUE`, `CHECK`, `PRIMARY KEY`, `FOREIGN KEY`.
   - Constraints enforce specific behavior (e.g., no duplicates, valid ranges).

### 3. **Denormalization**
   - Reduces table joins by merging tables, increasing query speed at the cost of data redundancy.
   - Useful in reporting and data warehousing.

### 4. **Primary Key**
   - Uniquely identifies each record in a table.
   - Cannot have `NULL` values.
   - Only one primary key per table, which may span multiple columns (composite key).

### 5. **Unique Key**
   - Ensures all values in a column are unique.
   - Allows one `NULL` value per column, unlike the primary key.

### 6. **Foreign Key**
   - Links records from two tables to enforce relationships.
   - References a primary key in another table, maintaining referential integrity.

### 7. **DELETE vs. TRUNCATE**
   - **DELETE**: Removes specific rows, can be rolled back.
   - **TRUNCATE**: Removes all rows quickly, cannot be rolled back.

### 8. **Clustered vs. Non-clustered Index**
   - **Clustered**: Orders data physically, only one allowed per table.
   - **Non-clustered**: Separate structure pointing to data rows, multiple allowed per table.

### 9. **Current Date Query**
   - MySQL: `SELECT CURDATE();`
   - SQL Server: `SELECT GETDATE();`
   - Returns the system's current date and time.

### 10. **Entities and Relationships**
   - **Entity**: Represents real-world objects, like `Employee`.
   - **Relationship**: Connects entities (e.g., `Employee` belongs to `Department`).

### 11. **Index**
   - A structure that speeds up data retrieval.
   - Types: **Unique**, **Clustered**, and **Non-clustered**.

### 12. **Normalization**
   - Process of organizing data to minimize redundancy.
   - Improves data integrity and reduces data anomalies.

### 13. **DROP vs. TRUNCATE**
   - **DROP**: Deletes the entire table structure and data.
   - **TRUNCATE**: Clears all data but retains table structure.

### 14. **Normalization Forms**
   - **1NF**: Atomic values.
   - **2NF**: Removes partial dependencies.
   - **3NF**: Removes transitive dependencies.
   - **BCNF**: Ensures every determinant is a candidate key.

### 15. **ACID Properties**
   - Key features for reliable transactions:
      - **Atomicity**: Transactions are all-or-nothing.
      - **Consistency**: Data remains valid.
      - **Isolation**: Transactions are independent.
      - **Durability**: Completed transactions are permanent.

### 16. **Trigger**
   - Automatically executed SQL code when specific table events occur.
   - Types: **BEFORE** and **AFTER** triggers.

### 17. **NULL Values**
   - `NULL` represents missing or unknown data.
   - Different from zero or empty spaces.

### 18. **Subquery**
   - A query within another query.
   - **Correlated**: References outer query.
   - **Non-correlated**: Runs independently of the outer query.

### 19. **Get Count of Records**
   - `SELECT COUNT(*) FROM table_name;`
   - Retrieves the total number of rows in a table.

### 20. **SQL Query for Third-Highest Salary**
   - `SELECT salary FROM employee ORDER BY salary DESC LIMIT 1 OFFSET 2;`
   - Ranks and retrieves a specific position in sorted data.

### 21. **Query for Names Starting with 'A'**
   - `SELECT name FROM employees WHERE name LIKE 'A%';`
   - Searches for names beginning with a specified letter.

### 22. **Group Functions**
   - Aggregate functions like `SUM`, `AVG`, and `COUNT` that operate on data groups.

### 23. **Relationship Types**
   - **One-to-One**, **One-to-Many**, **Many-to-Many**—link data across tables.

### 24. **Insert NULL Values**
   - Can omit columns or use `NULL` keyword explicitly.

### 25. **BETWEEN vs. IN Condition**
   - **BETWEEN**: Checks for range.
   - **IN**: Checks for matching values in a list.

### 26. **MERGE Statement**
   - Combines `INSERT`, `UPDATE`, and `DELETE` based on conditions.
   - Useful for synchronizing tables.

### 27. **Recursive Stored Procedure**
   - A stored procedure that calls itself.
   - Useful for hierarchical data.

### 28. **SQL Clause**
   - Commands like `WHERE`, `HAVING` that specify query conditions.

### 29. **HAVING vs. WHERE**
   - **WHERE**: Filters before grouping.
   - **HAVING**: Filters after grouping.

### 30. **Column vs. Table Level Constraints**
   - **Column Level**: Applies to individual columns.
   - **Table Level**: Applies to multiple columns.

### 31. **Fetch Common Records from Two Tables**
   - Use `JOIN` or `INTERSECT` to find common entries.

### 32. **Case Manipulation Functions**
   - **UPPER**: Converts to uppercase.
   - **LOWER**: Converts to lowercase.
   - **INITCAP**: Capitalizes the first letter of each word.

### 33. **Set Operators**
   - `UNION`, `INTERSECT`, `MINUS` for combining query results.

### 34. **Aggregate vs. Scalar Functions**
   - **Aggregate**: Works on groups (e.g., `SUM`).
   - **Scalar**: Works on single values (e.g., `ROUND`).

### 35. **Fetch Alternate Records**
   - Use `ROW_NUMBER()` or specific conditions based on ID.

### 36. **Select Unique Records**
   - `SELECT DISTINCT column_name FROM table_name;`

### 37. **Fetch First 5 Characters of a String**
   - `SUBSTRING(column_name, 1, 5);`

### 38. **View**
   - A virtual table based on a query.
   - Simplifies complex queries by encapsulating logic.

### 39. **Stored Procedure**
   - Predefined SQL statements.
   - **Advantages**: Reusable, efficient.
   - **Disadvantages**: Complexity, maintenance overhead.

### 40. **Collation**
   - Set of rules for sorting/comparing text.
   - Sensitivity types:
      - **Case** (e.g., A vs. a)
      - **Kana** (Japanese Kana differences)
      - **Width** (Single-byte vs. double-byte)
      - **Accent** (e.g., é vs. e)

### 41. **Local and Global Variables**
   - **Local**: Declared within functions, limited scope.
   - **Global**: Declared outside functions, broader scope.

### 42. **Auto Increment**
   - Automatically generates unique values for each row.
   - Used in primary keys.

### 43. **Data Warehouse**
   - Central repository for historical data.
   - Supports reporting and analysis.

### 44. **Authentication Modes in SQL Server**
   - **Windows Mode**: Uses Windows credentials.
   - **Mixed Mode**: Supports both SQL and Windows authentication.

### 45. **STUFF and REPLACE Functions**
   - **STUFF**: Inserts a substring at a specified position.
   - **REPLACE**: Replaces characters within a string.

### 46. **SQL Query to Get the Third-Highest Salary**
   - `SELECT salary FROM employees ORDER BY salary DESC LIMIT 1 OFFSET 2;`
   - This query fetches the salary at the third position after sorting in descending order.

### 47. **Group Functions in SQL**
   - Functions that operate on a set of rows, returning a single result.
   - Examples: `SUM`, `COUNT`, `AVG`, `MIN`, `MAX`.

### 48. **What is a Relationship in SQL?**
   - A way to link tables to define dependencies between data.
   - Types: **One-to-One**, **One-to-Many**, **Many-to-Many**.

### 49. **How to Insert NULL Values in SQL**
   - Can insert implicitly by omitting the column or explicitly using `NULL` keyword.
   - Example: `INSERT INTO table_name (column1) VALUES (NULL);`

### 50. **`BETWEEN` vs. `IN` Condition Operators**
   - **BETWEEN**: Checks if a value falls within a range.
     - Example: `WHERE age BETWEEN 20 AND 30`
   - **IN**: Checks if a value exists within a list.
     - Example: `WHERE color IN ('red', 'blue')`

### 51. **MERGE Statement**
   - Used to combine `INSERT`, `UPDATE`, and `DELETE` actions based on a condition.
   - Efficiently synchronizes tables by performing multiple operations in one statement.

### 52. **Recursive Stored Procedure**
   - A stored procedure that calls itself.
   - Useful for hierarchical or nested data (like org charts).

### 53. **Clause in SQL**
   - Keywords that define conditions for SQL queries.
   - Examples: `WHERE`, `GROUP BY`, `ORDER BY`, `HAVING`.

### 54. **`HAVING` Clause vs. `WHERE` Clause**
   - **WHERE**: Filters rows before grouping.
   - **HAVING**: Filters groups after `GROUP BY`.

### 55. **Column-Level vs. Table-Level Constraints**
   - **Column-Level**: Constraint applied to a single column.
   - **Table-Level**: Constraint applied across multiple columns (e.g., composite keys).

### 56. **Fetch Common Records from Two Tables**
   - Use `JOIN` or `INTERSECT` to find common records.
   - Example: `SELECT * FROM table1 INTERSECT SELECT * FROM table2;`

### 57. **Case Manipulation Functions in SQL**
   - Convert the case of text data.
   - **UPPER**: All uppercase, **LOWER**: All lowercase, **INITCAP**: Capitalizes first letter.

### 58. **Set Operators in SQL**
   - Combine results of two or more queries.
   - Examples: `UNION`, `INTERSECT`, `MINUS`.

### 59. **Aggregate vs. Scalar Functions**
   - **Aggregate Functions**: Operate on a set of values and return a single result (`SUM`, `AVG`).
   - **Scalar Functions**: Operate on individual values (`ROUND`, `LEN`).

### 60. **Fetch Alternate Records from a Table**
   - Use row number or ID patterns to select alternate rows.
   - Example with `MOD`: `SELECT * FROM table WHERE MOD(id, 2) = 0;`

### 61. **Select Unique Records from a Table**
   - Use `DISTINCT` keyword.
   - Example: `SELECT DISTINCT column_name FROM table_name;`

### 62. **Fetch First 5 Characters of a String**
   - Use `SUBSTRING` or `LEFT`.
   - Example: `SELECT SUBSTRING(column_name, 1, 5) FROM table_name;`

### 63. **View in SQL**
   - A virtual table based on a SQL query.
   - Simplifies complex queries, improves security, and makes data access easier.

### 64. **Stored Procedure with Advantages and Disadvantages**
   - **Stored Procedure**: Predefined SQL code for reuse.
   - **Advantages**: Reusable, efficient, and secure.
   - **Disadvantages**: Can be complex, requires maintenance.

### 65. **Collation in SQL**
   - Defines rules for string comparison (e.g., case, accent).
   - Types include **Case Sensitivity**, **Accent Sensitivity**, **Kana Sensitivity**, **Width Sensitivity**.

### 66. **Local vs. Global Variables**
   - **Local Variables**: Defined within functions, limited scope.
   - **Global Variables**: Defined outside functions, accessible globally.

### 67. **Auto Increment in SQL**
   - Automatically increases the value of a column for each new record.
   - Used in primary key columns to uniquely identify each row.

### 68. **Data Warehouse**
   - A large storage system for historical data, optimized for analysis.
   - Supports business intelligence and reporting.

### 69. **Authentication Modes in SQL Server**
   - **Windows Mode**: Uses Windows credentials.
   - **Mixed Mode**: Supports both SQL Server and Windows authentication.

### 70. **`STUFF` and `REPLACE` Functions**
   - **STUFF**: Inserts a substring at a specified position within a string.
   - **REPLACE**: Replaces occurrences of a specified substring with another.

