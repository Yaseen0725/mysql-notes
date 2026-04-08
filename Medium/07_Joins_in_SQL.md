# Lesson 7: Joins in SQL

In this lesson, we will learn how to combine data from multiple tables using joins.

Joins are used to retrieve related data from two or more tables.

---

## Example Tables

### employee

| employee_id | name | department_id |
|---|---|---|
| 1 | Yaseen | 101 |
| 2 | Anas | 102 |
| 3 | Ayesha | 101 |

### department

| department_id | department_name |
|---|---|
| 101 | IT |
| 102 | HR |

---

## 1. INNER JOIN
Returns only matching rows from both tables.

```sql
SELECT e.name, d.department_name
FROM employee e
INNER JOIN department d
ON e.department_id = d.department_id;
```

---

## 2. LEFT JOIN
Returns all rows from the left table and matching rows from the right table.

```sql
SELECT e.name, d.department_name
FROM employee e
LEFT JOIN department d
ON e.department_id = d.department_id;
```

---

## 3. RIGHT JOIN
Returns all rows from the right table and matching rows from the left table.

```sql
SELECT e.name, d.department_name
FROM employee e
RIGHT JOIN department d
ON e.department_id = d.department_id;
```

---

## 4. FULL OUTER JOIN
Returns all rows from both tables.

```sql
SELECT e.name, d.department_name
FROM employee e
FULL OUTER JOIN department d
ON e.department_id = d.department_id;
```

---

## Simple Understanding

- `INNER JOIN` → common data  
- `LEFT JOIN` → all left + matching right  
- `RIGHT JOIN` → all right + matching left  
- `FULL JOIN` → all data from both tables  
