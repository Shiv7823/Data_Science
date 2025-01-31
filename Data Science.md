
![SQL Image](https://media.istockphoto.com/id/1673063844/vector/sql-dtabase-flat-design.jpg?s=612x612&w=0&k=20&c=t-YSg_Wl7z8nJwhqZ2e74p_8tY98XWrJlOG9Vmdb_HY=)



# What is SQL ?

SQL (Structured Query Language) is a standard language used to store, manipulate, and retrieve data in relational databases.<br>
It allows users to create, read, update, and delete (CRUD) data in databases.<br>

<br>
<br>

# Why SQL is Important in Data Science ?

SQL is used in Data science for different purposes like :
1. Data Extraction<br>
2. Data cleaning and website<br>
3. Data Aggregation and Summarization<br>
4. Joining multiple Data Sources<br>


<br>
<br>


**Create a database**
```sql
CREATE DATABASE database_name
```


1. **Select the database to use**

```sql
USE your_database_name;
```

2. **Create a table named Employees**

```sql
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    Name VARCHAR(50) NOT NULL,
    Department VARCHAR(50) NOT NULL,
    Salary DECIMAL(10,2) NOT NULL,
    Experience INT NOT NULL
);
```

3. **Insert data into Employees table**

```sql
INSERT INTO Employees (EmployeeID, Name, Department, Salary, Experience) VALUES
(1, 'Amit Sharma', 'IT', 75000, 5),
(2, 'Priya Verma', 'HR', 60000, 4),
(3, 'Rahul Singh', 'Finance', 80000, 6),
(4, 'Neha Gupta', 'Marketing', 55000, 3),
(5, 'Vikas Joshi', 'IT', 90000, 7),
(6, 'Sneha Roy', 'HR', 58000, 4),
(7, 'Rohan Mehta', 'Finance', 85000, 5),
(8, 'Pooja Nair', 'Marketing', 62000, 3),
(9, 'Akash Das', 'IT', 72000, 6),
(10, 'Meera Iyer', 'HR', 63000, 4);
```

4. **Add a new column (Bonus) to Employees table**

```sql
ALTER TABLE Employees ADD Bonus DECIMAL(10,2);
```

5. **Remove the Bonus column from Employees table**

```sql
ALTER TABLE Employees DROP COLUMN Bonus;
```

6. **Remove all records from Employees table without deleting the structure**

```sql
TRUNCATE TABLE Employees;
```

7. **Update salary of an employee with EmployeeID = 1**

```sql
UPDATE Employees SET Salary = 78000 WHERE EmployeeID = 1;
```

8. **Retrieve all records from Employees table**

```sql
SELECT * FROM Employees;
```

9. **Delete an employee record with EmployeeID = 5**

```sql
DELETE FROM Employees WHERE EmployeeID = 5;
```

10. **Get the minimum salary in Employees table**

```sql
SELECT MIN(Salary) FROM Employees;
```

11. **Get the maximum salary in Employees table**

```sql
SELECT MAX(Salary) FROM Employees;
```

12. **Get the total number of employees**

```sql
SELECT COUNT(*) FROM Employees;
```

13. **Get the total sum of all salaries**

```sql
SELECT SUM(Salary) FROM Employees;
```

14. **Get the average salary in Employees table**

```sql
SELECT AVG(Salary) FROM Employees;
```
