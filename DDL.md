# `DDL` : Data Definition Language

### `CREATE` 
```sql
CREATE Table Employee
(
    Employee_ID INT NOT NULL IDENTITY(1,1) PRIMARY KEY,  # IDENTITY(1,1) Start from 1 and Increment by 1 
    First_Name  NVARCHAR(60),
    Last_Name   NVARCHAR(60),
    Email       NVARCHAR(60)
)
```

### `INSERT`
```sql
INSERT INTO Employee(First_Name, Last_Name, Email)  # Employee_ID will increment automatically. 
VALUES('Kirankumar', 'Yadav', 'Kirankumaryadav@gmail.com')
```

### `ALTER`
Change the structure (Data type, column names, add or drop columns) of table.
```sql
ALTER Table Employee
DROP Column Email
```
```sql
ALTER Table Employee
ADD Age INT, Department NVARCHAR(50)
```
```sql
ALTER Table Employee
ALTER Column Country NVARCHAR(30)
```

### `TRUNCATE`
Delete data from the table, while retaining the structure of the table.
```sql
TRUNCATE Table Employee
DROP Column Email
```

### `DROP`
Delete the entire table data including structure and constraints.
```sql
DROP Table Employee
```
