# Lesson 4: Inserting Data in Table in SQL

In this lesson, we will learn how to insert data into a table.

---

## Insert Single Row

```sql
INSERT INTO employee (name, position, department, hire_date, salary)
VALUES ('Md Tauqeer Manzar', 'Software Engineer', 'IT', '2024-01-15', 65000.00);
```

---

## Insert Multiple Rows

```sql
INSERT INTO employee (name, position, department, hire_date, salary)
VALUES
    ('Md Tauqeer Manzar', 'Software Engineer', 'IT', '2024-01-15', 65000.00),
    ('Md Sarfraz', 'HR Manager', 'Human Resources', '2023-06-20', 72000.50),
    ('Mohd Yaseen', 'Java Developer', 'Backend Development', '2025-02-10', 85000.00),
    ('Md Saifullah', 'Data Analyst', 'Analytics', '2024-08-05', 58000.75),
    ('Janishar Alam', 'Project Manager', 'Management', '2022-11-01', 95000.00);
```

---

## View Inserted Data

```sql
SELECT * FROM employee;
```

---

## Output Example

| employee_id | name | position | department | hire_date | salary |
|---|---|---|---|---|---:|
| 1 | Md Tauqeer Manzar | Software Engineer | IT | 2024-01-15 | 65000.00 |
| 2 | Md Sarfraz | HR Manager | Human Resources | 2023-06-20 | 72000.50 |
| 3 | Mohd Yaseen | Java Developer | Backend Development | 2025-02-10 | 85000.00 |
| 4 | Md Saifullah | Data Analyst | Analytics | 2024-08-05 | 58000.75 |
| 5 | Janishar Alam | Project Manager | Management | 2022-11-01 | 95000.00 |
