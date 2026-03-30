# Difference Between DROP, DELETE, and TRUNCATE

| Feature | DELETE | TRUNCATE | DROP |
|---|---|---|---|
| **Purpose** | Removes specific rows from a table | Removes all rows from a table | Deletes the entire table |
| **WHERE Clause** | Supported | Not supported | Not applicable |
| **Rollback** | Can be rolled back | Can be rolled back (in PostgreSQL) | Can be rolled back (in PostgreSQL) |
| **Table Structure** | Remains unchanged | Remains unchanged | Removed completely |
| **Speed** | Slower | Faster | Fastest |
| **Auto Increment Reset** | Does not reset | Resets identity/serial sequence (if specified) | Table removed |
| **Data Recovery** | Possible with rollback | Possible with rollback | Table must be recreated |
| **Use Case** | Delete selected records | Remove all records quickly | Remove table permanently |

---

## 1. DELETE
Used to remove **specific rows** from a table.

```sql
DELETE FROM employee WHERE employee_id = 1;
```

This deletes only the row where `employee_id = 1`.

---

## 2. TRUNCATE
Used to remove **all rows** from a table, but keeps the table structure.

```sql
TRUNCATE TABLE employee;
```

Table remains, but all records are deleted.

---

## 3. DROP
Used to remove the **entire table structure and data** permanently.

```sql
DROP TABLE employee;
```

Both table and data are deleted.

---

## Simple Memory Trick
- **DELETE** → Delete rows
- **TRUNCATE** → Empty table
- **DROP** → Remove table
