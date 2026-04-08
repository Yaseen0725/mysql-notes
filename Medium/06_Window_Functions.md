# Lesson 6: Window Functions in SQL

In this lesson, we will learn about window functions used to perform calculations across a set of table rows related to the current row.

Unlike aggregate functions, window functions do not collapse rows.

---

## Syntax

```sql
function_name() OVER (
    PARTITION BY column_name
    ORDER BY column_name
)
```

---

## 1. ROW_NUMBER()
Assigns a unique row number to each row.

```sql
SELECT 
    name,
    salary,
    ROW_NUMBER() OVER (ORDER BY salary DESC) AS row_num
FROM employee;
```

---

## 2. RANK()
Assigns rank with gaps for duplicate values.

```sql
SELECT 
    name,
    salary,
    RANK() OVER (ORDER BY salary DESC) AS rank_num
FROM employee;
```

---

## 3. DENSE_RANK()
Assigns rank without gaps.

```sql
SELECT 
    name,
    salary,
    DENSE_RANK() OVER (ORDER BY salary DESC) AS dense_rank
FROM employee;
```

---

## 4. LEAD()
Returns the next row value.

```sql
SELECT 
    name,
    salary,
    LEAD(salary) OVER (ORDER BY salary) AS next_salary
FROM employee;
```

---

## 5. LAG()
Returns the previous row value.

```sql
SELECT 
    name,
    salary,
    LAG(salary) OVER (ORDER BY salary) AS previous_salary
FROM employee;
```

---

## Example with PARTITION BY

```sql
SELECT 
    name,
    department,
    salary,
    RANK() OVER (
        PARTITION BY department
        ORDER BY salary DESC
    ) AS dept_rank
FROM employee;
```

This ranks employees department-wise.

---

## Simple Understanding

- `ROW_NUMBER()` → unique numbering  
- `RANK()` → rank with gaps  
- `DENSE_RANK()` → rank without gaps  
- `LEAD()` → next row  
- `LAG()` → previous row  
