# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
CREATE TABLE empk(empid NUMBER,empname VARCHAR(10),dept VARCHAR(20),salary NUMBER);
 CREATE OR REPLACE PROCEDURE insert_empk_data AS
   BEGIN
   INSERT INTO empk(empid,empname,dept,salary)
   VALUES(1,'sonu','HR',100000);
   INSERT INTO empk(empid,empname,dept,salary)
   VALUES(2,'knn','IT',20000);
   INSERT INTO empk(empid,empname,dept,salary)
   VALUES(3,'abi','AP',30000);
   COMMIT;
   END;
    /
```
### CALL PROCEDURE
```
begin
insert_empk_data;
end;
/
```
### Display
```
select * from empk;

```

### Output:
### CREATE PROCEDURE:
![db1](https://github.com/21005688/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/94747031/50d848ac-23ef-40be-b907-4f6039b92866)
### CALL PROCEDURE:
![db2](https://github.com/21005688/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/94747031/97de4fd3-6cf4-45d4-9119-875f7408af9b)
### DISPLAY TABLE:
![db3](https://github.com/21005688/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/94747031/15c1b22f-959c-4ff3-8e89-38973bf80499)

### Result:
Thus a program To create a procedure using PL/SQL has been created successfully.
