# Lesson 5: Conditional Functions in SQL

In this lesson, we will learn about conditional functions used to apply logic in SQL queries.

---

## 1. CASE Statement
The `CASE` statement is used to apply conditional logic, similar to `if-else`.

```sql
SELECT 
    name,
    salary,
    CASE
        WHEN salary >= 80000 THEN 'High'
        WHEN salary >= 50000 THEN 'Medium'
        ELSE 'Low'
    END AS salary_category
FROM employee;
```

---

## 2. COALESCE()
The `COALESCE()` function returns the first non-null value.

```sql
SELECT 
    name,
    COALESCE(department, 'Not Assigned') AS department
FROM employee;
```

If `department` is `NULL`, it returns `'Not Assigned'`.

---

## 3. NULLIF()
The `NULLIF()` function returns `NULL` if both values are equal.

```sql
SELECT NULLIF(100, 100);
```

Output:

```sql
NULL
```

Example:

```sql
SELECT NULLIF(salary, 0)
FROM employee;
```

---

## Example

```sql
SELECT 
    name,
    CASE
        WHEN age >= 18 THEN 'Adult'
        ELSE 'Minor'
    END AS status
FROM student;
```

---

## Simple Understanding

- `CASE` → conditional logic  
- `COALESCE` → first non-null value  
- `NULLIF` → returns NULL if equal  
