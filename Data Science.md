1. **Create a table named Employees**

```sql
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    Name VARCHAR(50) NOT NULL,
    Department VARCHAR(50) NOT NULL,
    Salary DECIMAL(10,2) NOT NULL,
    Experience INT NOT NULL
);
```

2. **Insert data into Employees table**

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

3. **Add a new column (Bonus) to Employees table**

```sql
ALTER TABLE Employees ADD Bonus DECIMAL(10,2);
```

4. **Remove the Bonus column from Employees table**

```sql
ALTER TABLE Employees DROP COLUMN Bonus;
```

5. **Remove all records from Employees table without deleting the structure**

```sql
TRUNCATE TABLE Employees;
```

6. **Update salary of an employee with EmployeeID = 1**

```sql
UPDATE Employees SET Salary = 78000 WHERE EmployeeID = 1;
```

7. **Retrieve all records from Employees table**

```sql
SELECT * FROM Employees;
```

8. **Delete an employee record with EmployeeID = 5**

```sql
DELETE FROM Employees WHERE EmployeeID = 5;
```

9. **Get the minimum salary in Employees table**

```sql
SELECT MIN(Salary) FROM Employees;
```

10. **Get the maximum salary in Employees table**

```sql
SELECT MAX(Salary) FROM Employees;
```

11. **Get the total number of employees**

```sql
SELECT COUNT(*) FROM Employees;
```

12. **Get the total sum of all salaries**

```sql
SELECT SUM(Salary) FROM Employees;
```

13. **Get the average salary in Employees table**

```sql
SELECT AVG(Salary) FROM Employees;
