# Lesson 9: Alter Column and Data Type in SQL

In this lesson, we will learn how to modify table columns and change data types using the `ALTER TABLE` statement.

---

## 1. Add a New Column

```sql
ALTER TABLE employee
ADD COLUMN email VARCHAR(100);
```

This adds a new column named `email`.

---

## 2. Rename a Column

```sql
ALTER TABLE employee
RENAME COLUMN name TO full_name;
```

This renames the `name` column to `full_name`.

---

## 3. Change Data Type

```sql
ALTER TABLE employee
ALTER COLUMN salary TYPE NUMERIC(12,2);
```

This changes the data type of `salary`.

---

## 4. Set NOT NULL Constraint

```sql
ALTER TABLE employee
ALTER COLUMN department SET NOT NULL;
```

This makes the `department` column mandatory.

---

## 5. Drop NOT NULL Constraint

```sql
ALTER TABLE employee
ALTER COLUMN department DROP NOT NULL;
```

This removes the `NOT NULL` rule.

---

## 6. Drop a Column

```sql
ALTER TABLE employee
DROP COLUMN email;
```

This removes the `email` column permanently.

---

## Important Note
`ALTER TABLE` is used to modify the structure of an existing table.
