# Lesson 1: SQL Functions

In this lesson, we will learn about commonly used SQL functions.

---

## 1. Aggregate Functions
Used to perform calculations on multiple rows.

| Function | Description | Example |
|---|---|---|
| `COUNT()` | Counts rows | `SELECT COUNT(*) FROM employee;` |
| `SUM()` | Adds values | `SELECT SUM(salary) FROM employee;` |
| `AVG()` | Average value | `SELECT AVG(salary) FROM employee;` |
| `MIN()` | Minimum value | `SELECT MIN(salary) FROM employee;` |
| `MAX()` | Maximum value | `SELECT MAX(salary) FROM employee;` |

---

## 2. String Functions

| Function | Description | Example |
|---|---|---|
| `UPPER()` | Converts to uppercase | `SELECT UPPER(name)` |
| `LOWER()` | Converts to lowercase | `SELECT LOWER(name)` |
| `LENGTH()` | Finds string length | `SELECT LENGTH(name)` |
| `CONCAT()` | Combines strings | `SELECT CONCAT(first_name, last_name)` |

---

## 3. Numeric Functions

| Function | Description | Example |
|---|---|---|
| `ROUND()` | Rounds number | `SELECT ROUND(123.456, 2)` |
| `CEIL()` | Round up | `SELECT CEIL(10.2)` |
| `FLOOR()` | Round down | `SELECT FLOOR(10.9)` |

---

## 4. Date Functions

| Function | Description | Example |
|---|---|---|
| `CURRENT_DATE` | Current date | `SELECT CURRENT_DATE;` |
| `CURRENT_TIME` | Current time | `SELECT CURRENT_TIME;` |
| `NOW()` | Current date and time | `SELECT NOW();` |
