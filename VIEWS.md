# Views

### Virtual Table (Do not Exist in Reality)

You can't `Modify` Data in the View.

### Columns = Fields 

### Rows = Records

- Selecting `Fields` | `Columns` from one or more Tables present in Database
- There is no `Records` | `Rows` in the View ( Only holds Definition of Table and Fetches Data from the Table and View it )


### CREATE VIEWS

```SQL
CREATE VIEW ViewName AS
SELECT Column1, Column2, Column3
FROM TablName
WHERE Conditions;
```

### Single Table
```SQL
CREATE VIEW Details AS
SELECT Name, Address
FROM Students 
WHERE Age > 18;
```

We can also Add GROUP BY, HAVING, ORDER BY...

### Multiple Table
```SQL
CREATE VIEW Details AS
SELECT S.Name, S.Address, M.Marks
FROM Students S, Marks M
WHERE S.ID = M.ID
```

### DROP VIEWS
```SQL
DROP VIEW Details
```
