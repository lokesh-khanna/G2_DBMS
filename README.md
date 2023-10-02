# EXP NO 1: DATA DEFINITION LANGUGE COMMANDS IN RDBMS

## AIM:
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.
</div>
 
## List of DDL commands: 
<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.
</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.
### SQL QUERY: 
```
CREATE TABLE student(
    rollno numeric(5),name char(50),age numeric(5),
    address varchar(100),
    phoneno numeric(10)
    );
```
### OUTPUT:
![image](https://github.com/lokesh-khanna/G2_DBMS/assets/119606216/544402cc-c984-41e7-ba98-24121788e359)

### 2) Change the above student table by adding another attribute department
### SQL QUERY: 
```
ALTER TABLE student ADD Department char(10);
```
### OUTPUT:
![image](https://github.com/lokesh-khanna/G2_DBMS/assets/119606216/7ed04220-8fbb-45bd-b857-8129d6d0701b)
### 3) Drop the student table
 ### SQL QUERY: 
```
DROP TABLE student;
```
![image](https://github.com/lokesh-khanna/G2_DBMS/assets/119606216/5bf3a6b2-5833-4a67-be00-3a05f710dc35)
### OUTPUT:
### 4) Delete the student table using truncate keyword
### SQL QUERY: 
```
TRUNCATE TABLE student;
```
### OUTPUT:
![image](https://github.com/lokesh-khanna/G2_DBMS/assets/119606216/60ebf97a-b3e8-4cbe-8b26-baa68bf0a335)
### 5) Rename the student table to mystudent
### SQL QUERY: 
```
ALTER TABLE student RENAME TO mystudent;
```
### OUTPUT:
![image](https://github.com/lokesh-khanna/G2_DBMS/assets/119606216/e04fc8a9-2510-4a6f-a6b8-a12375552dca)
### RESULT:
Thus a student database has been created and DDL queries are executed successfully.
