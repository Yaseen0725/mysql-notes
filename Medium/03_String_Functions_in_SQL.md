# Lesson 3: String Functions in SQL

In this lesson, we will learn about commonly used string functions in SQL.

---

## 1. UPPER()
Converts text to uppercase.

```sql
SELECT UPPER(name) FROM employee;
```

---

## 2. LOWER()
Converts text to lowercase.

```sql
SELECT LOWER(name) FROM employee;
```

---

## 3. LENGTH()
Returns the length of a string.

```sql
SELECT LENGTH(name) FROM employee;
```

---

## 4. CONCAT()
Combines multiple strings.

```sql
SELECT CONCAT(name, ' - ', department) FROM employee;
```

---

## 5. SUBSTRING()
Extracts a part of a string.

```sql
SELECT SUBSTRING(name, 1, 3) FROM employee;
```

---

## 6. TRIM()
Removes extra spaces from both sides.

```sql
SELECT TRIM(name) FROM employee;
```

---

## 7. REPLACE()
Replaces a part of a string.

```sql
SELECT REPLACE(name, 'a', 'x') FROM employee;
```

---

## 8. POSITION()
Finds position of substring.

```sql
SELECT POSITION('a' IN name) FROM employee;
```

---

## Example

```sql
SELECT 
    UPPER(name),
    LENGTH(name),
    CONCAT(name, ' works in ', department)
FROM employee;
```

---

## Simple Understanding

- `UPPER/LOWER` → change case  
- `LENGTH` → count characters  
- `CONCAT` → join strings  
- `SUBSTRING` → extract part  
- `TRIM` → remove spaces  
- `REPLACE` → change text  
