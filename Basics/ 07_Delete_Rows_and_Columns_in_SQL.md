# Lesson 7: Delete Rows and Columns in SQL

In this lesson, we will learn how to delete rows and columns from a table in PostgreSQL.

---

## Delete a Row
To delete specific rows from a table, use the `DELETE` statement.

```sql
DELETE FROM employee
WHERE employee_id = 1;
```

This deletes the row where `employee_id = 1`.

---

## Delete Multiple Rows
```sql
DELETE FROM employee
WHERE department = 'IT';
```

This deletes all employees from the IT department.

---

## Delete a Column
To remove a column from a table, use the `ALTER TABLE` statement with `DROP COLUMN`.

```sql
ALTER TABLE employee
DROP COLUMN salary;
```

This removes the `salary` column from the table permanently.

---

## Important Note
- `DELETE` → removes **rows**
- `DROP COLUMN` → removes **column structure**
