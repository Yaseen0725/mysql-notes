# Lesson 10: SELECT Query in SQL

In this lesson, we will learn how to retrieve data from a table using the `SELECT` statement.

---

## 1. Select All Data

```sql
SELECT * FROM employee;
```

This fetches all rows and columns from the `employee` table.

---

## 2. Select Specific Columns

```sql
SELECT name, department, salary
FROM employee;
```

This fetches only selected columns.

---

## 3. Select with Condition

```sql
SELECT *
FROM employee
WHERE department = 'IT';
```

This returns only employees from the IT department.

---

## 4. Select Distinct Values

```sql
SELECT DISTINCT department
FROM employee;
```

This removes duplicate department values.

---

## 5. Select with Sorting

```sql
SELECT *
FROM employee
ORDER BY salary DESC;
```

This sorts data by salary in descending order.

---

## 6. Limit Rows

```sql
SELECT *
FROM employee
LIMIT 5;
```

This returns only the first 5 rows.

---

## Important Note
`SELECT` is used to read or fetch data from the database.
