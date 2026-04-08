# Lesson 11: Types of Operators in SQL

In this lesson, we will learn about different types of operators used in SQL.

---

## 1. Arithmetic Operators
Used to perform mathematical operations.

| Operator | Description | Example |
|---|---|---|
| `+` | Addition | `SELECT 10 + 5;` |
| `-` | Subtraction | `SELECT 10 - 5;` |
| `*` | Multiplication | `SELECT 10 * 5;` |
| `/` | Division | `SELECT 10 / 5;` |
| `%` | Modulus | `SELECT 10 % 3;` |

---

## 2. Comparison Operators
Used to compare values.

| Operator | Description | Example |
|---|---|---|
| `=` | Equal to | `WHERE age = 25` |
| `!=` / `<>` | Not equal | `WHERE age != 25` |
| `>` | Greater than | `WHERE salary > 50000` |
| `<` | Less than | `WHERE salary < 50000` |
| `>=` | Greater than or equal | `WHERE age >= 18` |
| `<=` | Less than or equal | `WHERE age <= 60` |

---

## 3. Logical Operators
Used to combine conditions.

| Operator | Description | Example |
|---|---|---|
| `AND` | Both conditions must be true | `WHERE age > 18 AND salary > 50000` |
| `OR` | Any one condition must be true | `WHERE department = 'IT' OR department = 'HR'` |
| `NOT` | Negates a condition | `WHERE NOT department = 'IT'` |

---

## 4. Special Operators

### IN
```sql
SELECT * FROM employee
WHERE department IN ('IT', 'HR');
```

### BETWEEN
```sql
SELECT * FROM employee
WHERE salary BETWEEN 30000 AND 80000;
```

### LIKE
```sql
SELECT * FROM employee
WHERE name LIKE 'A%';
```

### IS NULL
```sql
SELECT * FROM employee
WHERE department IS NULL;
```

---

## Simple Understanding
- Arithmetic → calculations
- Comparison → comparisons
- Logical → multiple conditions
- Special → advanced filtering
