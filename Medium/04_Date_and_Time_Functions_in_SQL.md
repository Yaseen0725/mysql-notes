# Lesson 4: Date and Time Functions in SQL

In this lesson, we will learn about commonly used date and time functions in SQL.

---

## 1. CURRENT_DATE
Returns the current system date.

```sql
SELECT CURRENT_DATE;
```

Example output:

```sql
2026-04-09
```

---

## 2. CURRENT_TIME
Returns the current system time.

```sql
SELECT CURRENT_TIME;
```

Example output:

```sql
23:45:10.123456+05:30
```

---

## 3. NOW()
Returns the current date and time.

```sql
SELECT NOW();
```

Example output:

```sql
2026-04-09 23:45:10.123456+05:30
```

---

## 4. AGE()
Returns the difference between two dates.

```sql
SELECT AGE('2026-04-09', '2002-01-15');
```

---

## 5. EXTRACT()
Extracts a specific part from date/time.

```sql
SELECT EXTRACT(YEAR FROM CURRENT_DATE);
SELECT EXTRACT(MONTH FROM CURRENT_DATE);
SELECT EXTRACT(DAY FROM CURRENT_DATE);
```

---

## 6. DATE_PART()
Similar to EXTRACT, returns a part of date.

```sql
SELECT DATE_PART('year', NOW());
```

---

## 7. TO_CHAR()
Formats date and time as text.

```sql
SELECT TO_CHAR(NOW(), 'DD-MM-YYYY');
SELECT TO_CHAR(NOW(), 'HH24:MI:SS');
```

---

## Example

```sql
SELECT 
    CURRENT_DATE,
    CURRENT_TIME,
    NOW(),
    EXTRACT(YEAR FROM NOW());
```

---

## Simple Understanding

- `CURRENT_DATE` → current date  
- `CURRENT_TIME` → current time  
- `NOW()` → date + time  
- `AGE()` → date difference  
- `EXTRACT()` → specific part  
- `TO_CHAR()` → formatting  
