# Task 2: Data Insertion and Handling Nulls

## 📌 Objective
The goal of this task is to practice working with SQL Data Manipulation Language (DML) commands such as `INSERT`, `UPDATE`, and `DELETE`. It also demonstrates how to handle `NULL` values during data operations.

---

## 📁 Files Included

- `task2_data_handling.sql`  
  Contains SQL statements for:
  - Table creation
  - Inserting data (with and without NULLs)
  - Updating values including handling NULLs
  - Deleting specific records based on conditions

---

## 📝 Description of SQL Operations

### 1. Table Creation
Creates a table named `Employees` with the following fields:
- `EmpID` (Primary Key)
- `Name`
- `Department`
- `Salary`
- `Email`

### 2. Data Insertion
- Inserts 4 records into the `Employees` table.
- Includes examples with `NULL` values for fields like `Department`, `Salary`, `Email`, and `Name`.

### 3. Update Operations
- Updates specific fields where `NULL` values exist.
- Assigns default values to `NULL` fields such as:
  - Setting a missing department
  - Providing a salary for an employee
  - Replacing a NULL name with `"Unnamed"`

### 4. Delete Operation
- Deletes records where `Salary` is either `NULL` or less than 30,000.

---

## 🚀 How to Run

1. Open your preferred SQL environment (e.g., MySQL Workbench, pgAdmin, SQLite).
2. Run the contents of `task2_data_handling.sql`.
3. Optionally, run:
   ```sql
   SELECT * FROM Employees;
