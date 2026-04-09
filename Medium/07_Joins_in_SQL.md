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
Returns only the matching records from both tables.

<img width="512" height="290" alt="Inner Join" src="https://github.com/user-attachments/assets/8cf8939c-d72a-451c-9e4e-0cfaf920c9b3" />

```sql
SELECT e.name, d.department_name
FROM employee e
INNER JOIN department d
ON e.department_id = d.department_id;
```

---

## 2. LEFT JOIN
Returns all records from the left table and matching records from the right table.

<img width="512" height="290" alt="Left Join" src="https://github.com/user-attachments/assets/ac38bbbb-ac5e-418e-9940-11c349237bdf" />

```sql
SELECT e.name, d.department_name
FROM employee e
LEFT JOIN department d
ON e.department_id = d.department_id;
```

---

## 3. RIGHT JOIN
Returns all records from the right table and matching records from the left table.

<img width="512" height="290" alt="Right Join" src="https://github.com/user-attachments/assets/3feac5b5-0541-43d0-bdb1-024310a79384" />

```sql
SELECT e.name, d.department_name
FROM employee e
RIGHT JOIN department d
ON e.department_id = d.department_id;
```

---

## 4. FULL JOIN
Returns all records from both tables.

<img width="512" height="290" alt="Full Join" src="https://github.com/user-attachments/assets/b69e90da-f533-480e-9833-de46086936ef" />

```sql
SELECT e.name, d.department_name
FROM employee e
FULL OUTER JOIN department d
ON e.department_id = d.department_id;
```

## Simple Understanding

- `INNER JOIN` → common data  
- `LEFT JOIN` → all left + matching right  
- `RIGHT JOIN` → all right + matching left  
- `FULL JOIN` → all data from both tables



