# Oracle Database Administration Assignment 2

**Student Name:** Mutaz  
**Student ID:** 31086  

---

## Task 1: Create a Pluggable Database (PDB)
In this task, a new pluggable database was successfully created along with an administrative user and granted full privileges.

### SQL Commands Executed:
```sql
CONNECT / AS SYSDBA;

CREATE PLUGGABLE DATABASE mz_pdb_31086 
ADMIN USER Mutaz_plsqlauca_31086 
IDENTIFIED BY Oracle123;

ALTER PLUGGABLE DATABASE mz_pdb_31086 OPEN;
ALTER SESSION SET CONTAINER = mz_pdb_31086;
GRANT CONNECT, RESOURCE, DBA TO Mutaz_plsqlauca_31086;
