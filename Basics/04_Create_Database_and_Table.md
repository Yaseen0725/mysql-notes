# Lesson 4: Create Database and Table in SQL

In this lesson, we will learn how to create a database and a table in SQL using PostgreSQL.

---

## Create Database

Use the following query to create a new database:

```sql
CREATE DATABASE company_db;
```

To use the database:

```sql
\c company_db
```

---

## Create Table

The following query creates an `employee` table:

```sql
CREATE TABLE employee (
    employee_id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    position VARCHAR(50),
    department VARCHAR(50),
    hire_date DATE,
    salary NUMERIC(10,2)
);
```

---

## Explanation

- `SERIAL` → Auto-incrementing primary key
- `PRIMARY KEY` → Unique identifier
- `VARCHAR(50)` → Stores text up to 50 characters
- `NOT NULL` → Value cannot be empty
- `DATE` → Stores date
- `NUMERIC(10,2)` → Stores decimal salary values

---

## Verify Table

```sql
SELECT * FROM employee;
```
