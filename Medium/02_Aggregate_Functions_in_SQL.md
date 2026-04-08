# Lesson 2: Aggregate Functions in SQL

In this lesson, we will learn about aggregate functions used to perform calculations on multiple rows of data.

---

## 1. COUNT()
Returns the total number of rows.

```sql
SELECT COUNT(*) FROM employee;
```

---

## 2. SUM()
Returns the total sum of numeric values.

```sql
SELECT SUM(salary) FROM employee;
```

---

## 3. AVG()
Returns the average value.

```sql
SELECT AVG(salary) FROM employee;
```

---

## 4. MIN()
Returns the minimum value.

```sql
SELECT MIN(salary) FROM employee;
```

---

## 5. MAX()
Returns the maximum value.

```sql
SELECT MAX(salary) FROM employee;
```

---

## Example with GROUP BY

```sql
SELECT department, AVG(salary)
FROM employee
GROUP BY department;
```

This returns average salary department-wise.

---

## Example Output

| department | avg_salary |
|---|---:|
| IT | 65000 |
| HR | 72000 |
| Management | 95000 |

---

## Simple Understanding

- `COUNT()` → count rows  
- `SUM()` → add values  
- `AVG()` → average  
- `MIN()` → smallest  
- `MAX()` → largest  
