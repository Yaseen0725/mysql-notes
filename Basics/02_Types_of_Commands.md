
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

- **DDL (Data Definition Language)**  
  Used to **define and manage the structure** of the database, such as creating, modifying, or deleting tables and other database objects.  
  **Examples:** `CREATE`, `ALTER`, `DROP`, `TRUNCATE`

- **DML (Data Manipulation Language)**  
  Used to **insert, update, and delete data** stored inside database tables.  
  **Examples:** `INSERT`, `UPDATE`, `DELETE`

- **TCL (Transaction Control Language)**  
  Used to **manage transactions** in the database, allowing changes to be saved or undone.  
  **Examples:** `COMMIT`, `ROLLBACK`, `SAVEPOINT`

- **DCL (Data Control Language)**  
  Used to **control user access and permissions** in the database.  
  **Examples:** `GRANT`, `REVOKE`

- **DQL (Data Query Language)**  
  Used to **retrieve data** from the database.  
  **Examples:** `SELECT`
