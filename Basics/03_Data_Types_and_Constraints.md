# Lesson 3: Data Types and Constraints in SQL

In this lesson, we will learn about **SQL data types** and **constraints**.

---

## 1. Data Types in SQL
Data types define the **kind of value** that a column can store.

### Common Data Types

| Data Type | Description | Example |
|---|---|---|
| `INT` | Stores integer values | `25` |
| `VARCHAR(n)` | Stores variable-length strings | `'Yaseen'` |
| `CHAR(n)` | Fixed-length string | `'A'` |
| `DATE` | Stores date values | `'2025-04-06'` |
| `TIME` | Stores time values | `'10:30:00'` |
| `TIMESTAMP` | Stores date and time | `'2025-04-06 10:30:00'` |
| `BOOLEAN` | Stores true/false values | `TRUE` |
| `NUMERIC(p,s)` | Decimal numbers | `50000.75` |

---

## Example
```sql
CREATE TABLE student (
    id SERIAL,
    name VARCHAR(50),
    age INT,
    joining_date DATE,
    fee NUMERIC(10,2)
);
```

---

## 2. Constraints in SQL
Constraints are rules applied to columns to maintain **data integrity**.

### Common Constraints

| Constraint | Description |
|---|---|
| `NOT NULL` | Column cannot contain NULL values |
| `UNIQUE` | All values must be unique |
| `PRIMARY KEY` | Unique identifier for each row |
| `FOREIGN KEY` | Links one table to another |
| `CHECK` | Validates a condition |
| `DEFAULT` | Sets a default value |
| `AUTO_INCREMENT / SERIAL` | Auto-generates values |

---

## Example
```sql
CREATE TABLE student (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE,
    age INT CHECK (age >= 18),
    department VARCHAR(50) DEFAULT 'CSE'
);
```

---

## Simple Understanding
- **Data Types** → what type of data is stored
- **Constraints** → rules applied on data
