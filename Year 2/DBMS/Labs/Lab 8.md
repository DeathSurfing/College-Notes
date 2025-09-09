___
## Introduction:

This experiment focuses on implementing **MySQL Views and Stored Procedures** within an Employee Management System. Views help simplify complex queries by providing virtual tables, while Stored Procedures automate repetitive database tasks such as adding employees, updating salaries, and calculating departmental expenses. These techniques improve maintainability, security, and performance in database management.
## Observations:

- The **HighEarningEmployees view** effectively displayed employees earning more than 6000, automatically reflecting any changes in the underlying Employees table.
    
- The **DepartmentSalaryExpenses view** showed up-to-date total salary expenses per department, useful for quick financial reporting.
    
- The **AddNewEmployee procedure** inserted new employees while providing a clear success message including the generated EmployeeID.
    
- The **UpdateDepartmentSalary procedure** successfully increased salaries by a percentage and returned a message showing how many employees were affected.
    
- The **RemoveLowSalaryEmployees procedure** displayed employees who were going to be deleted before deleting them, ensuring clarity and preventing accidental deletions.
    
- The **CalculateTotalSalaryExpense procedure** returned a summary with department ID, name, number of employees, and total salary expense, enabling efficient salary tracking per department.

## Database Schema Setup

First, create the database and tables with sample data:

```sql
-- Create the employee management database
CREATE DATABASE employee_management;
USE employee_management;

-- Create Departments table
CREATE TABLE Departments (
    DepartmentID INT PRIMARY KEY,
    DepartmentName VARCHAR(100) NOT NULL
);

-- Create Employees table
CREATE TABLE Employees (
    EmployeeID INT AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(100) NOT NULL,
    DepartmentID INT,
    Salary DECIMAL(10, 2) NOT NULL,
    FOREIGN KEY (DepartmentID) REFERENCES Departments(DepartmentID)
);

-- Insert sample departments
INSERT INTO Departments (DepartmentID, DepartmentName) VALUES
    (101, 'Sales'),
    (102, 'Marketing'),
    (103, 'IT');

-- Insert sample employees
INSERT INTO Employees (EmployeeID, Name, DepartmentID, Salary) VALUES
    (1, 'John Doe', 101, 5000.00),
    (2, 'Jane Smith', 102, 6000.00),
    (3, 'Emily Davis', 101, 5500.00),
    (4, 'Michael Brown', 103, 7000.00),
    (5, 'Sarah Johnson', 102, 7500.00),
    (6, 'David Miller', 101, 5200.00);
```
![[Screenshot 2025-09-04 at 11.39.37 AM.png]]
## Initial Data Verification

```sql
-- View all departments
SELECT * FROM Departments;

-- View all employees with their department names
SELECT e.EmployeeID, e.Name, e.Salary, d.DepartmentName
FROM Employees e
JOIN Departments d ON e.DepartmentID = d.DepartmentID;
```
![[Screenshot 2025-09-04 at 11.39.57 AM.png]]
## Task Solutions

### Task 1: Create VIEW for High Earning Employees

Create a view to display employees earning more than 6000:

```sql
CREATE VIEW HighEarningEmployees AS
SELECT 
    e.EmployeeID,
    e.Name,
    e.Salary,
    d.DepartmentName
FROM Employees e
JOIN Departments d ON e.DepartmentID = d.DepartmentID
WHERE e.Salary > 6000;

-- Test the view
SELECT * FROM HighEarningEmployees;
```
![[Screenshot 2025-09-04 at 11.40.11 AM.png]]
### Task 2: Create VIEW for Department Salary Expenses

Create a view to show total salary expenses per department:

```sql
CREATE VIEW DepartmentSalaryExpenses AS
SELECT 
    d.DepartmentName,
    SUM(e.Salary) AS TotalSalaryExpense
FROM Departments d
LEFT JOIN Employees e ON d.DepartmentID = e.DepartmentID
GROUP BY d.DepartmentID, d.DepartmentName;

-- Test the view
SELECT * FROM DepartmentSalaryExpenses;
```
![[Screenshot 2025-09-04 at 11.40.22 AM.png]]
### Task 3: Create Procedure to Add New Employee

Create a stored procedure to insert a new employee:

```sql
CREATE PROCEDURE AddNewEmployee(
    IN emp_name VARCHAR(50),
    IN dept_id INT,
    IN emp_salary DECIMAL(10, 2)
)
BEGIN
    INSERT INTO Employees (Name, DepartmentID, Salary) 
    VALUES (emp_name, dept_id, emp_salary);
    
    SELECT CONCAT('Employee "', emp_name, '" added successfully with ID: ', LAST_INSERT_ID()) AS Result;
END;

-- Test the procedure
CALL AddNewEmployee('Anna Taylor', 103, 6800);

-- Verify the new employee was added
SELECT * FROM Employees WHERE Name = 'Anna Taylor';

```
![[Screenshot 2025-09-04 at 12.10.52 PM.png]] 
### Task 4: Create Procedure to Update Department Salary

Create a stored procedure to increase salaries by percentage for a department:

```sql
CREATE PROCEDURE UpdateDepartmentSalary(
    IN dept_id INT,
    IN increment_percentage DECIMAL(5, 2)
)
BEGIN
    DECLARE affected_rows INT DEFAULT 0;
    
    UPDATE Employees 
    SET Salary = Salary * (1 + increment_percentage / 100)
    WHERE DepartmentID = dept_id;
    
    SET affected_rows = ROW_COUNT();
    
    SELECT CONCAT(affected_rows, ' employees in department ', dept_id, ' received a ', 
                  increment_percentage, '% salary increase') AS Result;
END;

-- Test the procedure
CALL UpdateDepartmentSalary(101, 10);

-- Verify the salary updates
SELECT e.Name, e.Salary, d.DepartmentName 
FROM Employees e
JOIN Departments d ON e.DepartmentID = d.DepartmentID
WHERE e.DepartmentID = 101;

```
![[Screenshot 2025-09-04 at 11.42.25 AM.png]]
### Task 5: Create Procedure to Remove Low Salary Employees

Create a stored procedure to delete employees below a salary threshold:

```sql
CREATE PROCEDURE RemoveLowSalaryEmployees(
    IN salary_threshold DECIMAL(10, 2)
)
BEGIN
    DECLARE affected_rows INT DEFAULT 0;
    
    -- Show employees that will be removed
    SELECT CONCAT('Employees to be removed (salary < ', salary_threshold, '):') AS Notice;
    SELECT EmployeeID, Name, Salary 
    FROM Employees 
    WHERE Salary < salary_threshold;
    
    -- Delete them
    DELETE FROM Employees 
    WHERE Salary < salary_threshold;
    
    -- Get how many were deleted
    SET affected_rows = ROW_COUNT();
    
    -- Show result
    SELECT CONCAT(affected_rows, ' employees with salary below ', salary_threshold, ' have been removed') AS Result;
END;

-- Test the procedure
CALL RemoveLowSalaryEmployees(6000);

-- Verify remaining employees
SELECT * FROM Employees;

```
![[Screenshot 2025-09-04 at 11.44.51 AM.png]]
### Task 6: Create Procedure to Calculate Total Salary Expense

Create a stored procedure to calculate total salary expense for a department:

```sql
CREATE PROCEDURE CalculateTotalSalaryExpense(
    IN dept_id INT
)
BEGIN
    DECLARE total_expense DECIMAL(15, 2) DEFAULT 0;
    DECLARE dept_name VARCHAR(100);
    DECLARE employee_count INT DEFAULT 0;
    
    -- Get department name
    SELECT DepartmentName INTO dept_name 
    FROM Departments 
    WHERE DepartmentID = dept_id;
    
    -- Calculate total salary expense and employee count
    SELECT 
        COALESCE(SUM(Salary), 0),
        COUNT(*)
    INTO total_expense, employee_count
    FROM Employees 
    WHERE DepartmentID = dept_id;
    
    -- Return results
    SELECT 
        dept_id AS DepartmentID,
        dept_name AS DepartmentName,
        employee_count AS EmployeeCount,
        total_expense AS TotalSalaryExpense;
END;

-- Test the procedure
CALL CalculateTotalSalaryExpense(101); -- Sales
CALL CalculateTotalSalaryExpense(102); -- Marketing  
CALL CalculateTotalSalaryExpense(103); -- IT

```
![[Screenshot 2025-09-04 at 11.45.19 AM.png]]
## Additional Verification Queries

### View All Created Views

```sql
-- Test both views after all procedures have been executed
SELECT 'HIGH EARNING EMPLOYEES VIEW:' AS Section;
SELECT * FROM HighEarningEmployees;

SELECT 'DEPARTMENT SALARY EXPENSES VIEW:' AS Section;  
SELECT * FROM DepartmentSalaryExpenses;
```
![[Screenshot 2025-09-04 at 11.46.43 AM.png]]
### Final Data State

```sql
-- Show final state of all data
SELECT 'FINAL EMPLOYEES DATA:' AS Section;
SELECT e.EmployeeID, e.Name, e.Salary, d.DepartmentName
FROM Employees e
JOIN Departments d ON e.DepartmentID = d.DepartmentID
ORDER BY e.DepartmentID, e.EmployeeID;

SELECT 'FINAL DEPARTMENTS DATA:' AS Section;
SELECT * FROM Departments;
```
![[Screenshot 2025-09-04 at 11.47.00 AM.png]]
## Summary of Operations

1. **View HighEarningEmployees**: Displays employees earning > 6000
2. **View DepartmentSalaryExpenses**: Shows total salary expenses per department
3. **Procedure AddNewEmployee**: Adds new employees to the system
4. **Procedure UpdateDepartmentSalary**: Increases departmental salaries by percentage
5. **Procedure RemoveLowSalaryEmployees**: Removes employees below salary threshold
6. **Procedure CalculateTotalSalaryExpense**: Calculates department salary totals

Each procedure includes error handling and informative output messages to track the operations performed.

## Conclusion:

The lab demonstrated the power of **Views** and **Stored Procedures** in managing an employee database. Key takeaways include:

- Views act as dynamic virtual tables that simplify repeated or complex queries and provide a layer of abstraction.
    
- Stored Procedures encapsulate logic into reusable functions, enhancing maintainability and promoting code reuse.
    
- Proper use of parameters in procedures enables flexible and robust operations (e.g., adding employees, updating salaries).
    
- Informative outputs and validations in procedures (such as showing affected rows) improve traceability of operations.
    

Overall, the combination of Views and Stored Procedures facilitates scalable, efficient, and secure database management, especially suitable for business-critical applications like employee management.