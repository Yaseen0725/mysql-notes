
# 5 Types Commands in SQL

```mermaid
flowchart TB
    A[COMMANDS]
    H(( ))

    A --> H
    H --- B[DDL]
    H --- C[DML]
    H --- D[TCL]
    H --- E[DCL]
    H --- F[DQL]

    style A fill:#ff5c33,color:#fff,stroke:#000
    style B fill:#d2b48c,color:#000
    style C fill:#d2b48c,color:#000
    style D fill:#d2b48c,color:#000
    style E fill:#d2b48c,color:#000
    style F fill:#d2b48c,color:#000
    style H fill:none,stroke:none
```


  ## SQL Command Types

### 1. DDL (Data Definition Language)
DDL commands are used to **define, modify, and remove the structure of database objects** such as tables, schemas, indexes, and databases.

**Common Commands:**
- `CREATE` → Creates a new table, database, or object
- `ALTER` → Modifies the structure of an existing table
- `DROP` → Deletes a table or database permanently
- `TRUNCATE` → Removes all records from a table without deleting the table structure

---

### 2. DML (Data Manipulation Language)
DML commands are used to **manipulate the data stored inside database tables**.

**Common Commands:**
- `INSERT` → Adds new records into a table
- `UPDATE` → Modifies existing records
- `DELETE` → Removes specific records from a table

---

### 3. TCL (Transaction Control Language)
TCL commands are used to **manage transactions in the database**, ensuring data consistency and control over changes.

**Common Commands:**
- `COMMIT` → Saves all changes permanently
- `ROLLBACK` → Undoes changes made in the current transaction
- `SAVEPOINT` → Creates a point to which a transaction can be rolled back

---

### 4. DCL (Data Control Language)
DCL commands are used to **control access and permissions** for database users.

**Common Commands:**
- `GRANT` → Gives privileges to users
- `REVOKE` → Removes privileges from users

---

### 5. DQL (Data Query Language)
DQL commands are used to **retrieve data from the database**.

**Common Commands:**
- `SELECT` → Fetches data from one or more tables
