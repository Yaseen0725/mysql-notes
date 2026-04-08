# Lesson 6: Update Data in SQL

In this lesson, we will learn how to update existing data in a table using the `UPDATE` statement.

---

## Syntax

```sql
UPDATE table_name
SET column_name = value
WHERE condition;
```

---

## Example 1: Update a Single Row

```sql
UPDATE employee
SET salary = 70000
WHERE employee_id = 1;
```

This updates the salary of the employee whose `employee_id` is `1`.

---

## Example 2: Update Multiple Columns

```sql
UPDATE employee
SET department = 'IT',
    salary = 80000
WHERE employee_id = 2;
```

This updates both department and salary.

---

## Example 3: Update Multiple Rows

```sql
UPDATE employee
SET department = 'Engineering'
WHERE department = 'IT';
```

This updates all employees in the IT department.

---

## Important Note
Always use the `WHERE` clause.

Without `WHERE`, all rows will be updated.

```sql
UPDATE employee
SET salary = 50000;
```

This updates salary for every row in the table.
