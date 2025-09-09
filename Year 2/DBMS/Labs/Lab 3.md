
___

# Question 1:
 Create a table with student database in that student database mention , student_id, student_name, course_name, address, with the help of these data execute SQL query
 **Queries:**
 a) Select Distinct 
 b) and , or, not
 c) between
 d) Ordered by ascending, descending order
 e) isNULL
 f) select top 3 positions
 g) min value, max value, average, total students

## Create Table Students
```SQL
CREATE TABLE students (
    student_id INT PRIMARY KEY,
    student_name VARCHAR(100),
    course_name VARCHAR(100),
    address VARCHAR(255)
);

INSERT INTO students (student_id, student_name, course_name, address) VALUES
(1, 'Alice Johnson', 'Computer Science', 'New York'),
(2, 'Bob Smith', 'Business', 'Chicago'),
(3, 'Charlie Davis', 'Computer Science', 'New York'),
(4, 'David Wilson', 'Mathematics', 'Houston'),
(5, 'Eva Brown', 'Business', 'Boston'),
(6, 'Frank Taylor', NULL, 'Seattle'),
(7, 'Grace Miller', 'Computer Science', NULL),
(8, 'Hannah Lee', 'Mathematics', 'New York'),
(9, 'Ian Thomas', 'Business', 'Chicago'),
(10, 'Jack White', 'Computer Science', 'New York');
```


## SQL Queries

### A)

```SQL
SELECT DISTINCT course_name FROM students;
```
![[Screenshot 2025-07-24 at 10.46.42 AM.png]]


### B)
```sql
-- Students from New York who study Computer Science
SELECT * FROM students
WHERE address = 'New York' AND course_name = 'Computer Science';

-- Students who are either in Business or from Boston
SELECT * FROM students
WHERE course_name = 'Business' OR address = 'Boston';

-- Students who are NOT from Chicago
SELECT * FROM students
WHERE NOT address = 'Chicago';
```

![[Screenshot 2025-07-24 at 10.47.56 AM.png]]

### C)
```SQL
SELECT * FROM students
WHERE student_id BETWEEN 3 AND 7;
```
![[Screenshot 2025-07-24 at 10.48.46 AM.png]]

### D)

```SQL
-- Ascending order by student_name
SELECT * FROM students
ORDER BY student_name ASC;

-- Descending order by student_id
SELECT * FROM students
ORDER BY student_id DESC;
```

![[Screenshot 2025-07-24 at 10.49.38 AM.png]]

### E) 

```sql
-- Students without a course assigned
SELECT * FROM students
WHERE course_name IS NULL;

-- Students with a missing address
SELECT * FROM students
WHERE address IS NULL;
```

![[Screenshot 2025-07-24 at 10.50.20 AM.png]]


### F)
```SQL
SELECT * FROM students
ORDER BY student_id
LIMIT 3;
```
![[Screenshot 2025-07-24 at 10.51.03 AM.png]]

### G)
```SQL
-- Minimum student ID
SELECT MIN(student_id) AS min_id FROM students;
-- RETURNS 1

-- Maximum student ID
SELECT MAX(student_id) AS max_id FROM students;
-- REUTRNS 10

-- Average student ID
SELECT AVG(student_id) AS avg_id FROM students;
-- RETURNS 5.5000

-- Total number of students
SELECT COUNT(*) AS total_students FROM students;
-- RETURNS 10

```


# Question 2:

Managing a database for a car dealership company, the database should keep track of the cars available for sale , customers , sales transactions and sales representatives involved in each transaction add cars data, customer data, sales report and sales
 a) Select Distinct 
 b) and , or, not
 c) between
 d) Ordered by ascending, descending order
 e) isNULL
 f) select top 3 positions
 g) min value, max value, average, total students

### Cars Table:
```sql
CREATE TABLE Cars (
    CarID INT PRIMARY KEY,
    Make VARCHAR(50),
    Model VARCHAR(50),
    Year INT,
    Price DECIMAL(10, 2),
    Availability BOOLEAN
);
```
### Customers Table:
```sql
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    Email VARCHAR(100),
    Phone VARCHAR(15),
    Address VARCHAR(200)
);
```

### Sales Rep Table:
```sql
CREATE TABLE SalesReps (
    RepID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    Email VARCHAR(100),
    Phone VARCHAR(15)
);
```

### Sales Table:
```sql
CREATE TABLE Sales (
    SaleID INT PRIMARY KEY,
    CarID INT,
    CustomerID INT,
    RepID INT,
    SaleDate DATE,
    SalePrice DECIMAL(10, 2),
    FOREIGN KEY (CarID) REFERENCES Cars(CarID),
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID),
    FOREIGN KEY (RepID) REFERENCES SalesReps(RepID)
);
```

### Seed cars table
```sql
INSERT INTO Cars VALUES 
(1, 'Toyota', 'Camry', 2022, 25000.00, TRUE),
(2, 'Honda', 'Civic', 2021, 22000.00, TRUE),
(3, 'Ford', 'Mustang', 2023, 35000.00, TRUE),
(4, 'Tesla', 'Model 3', 2023, 40000.00, TRUE);
```

### Seed customers table
```sql
INSERT INTO Customers VALUES 
(1, 'John', 'Doe', 'john.doe@email.com', '1234567890', '123 Elm Street'),
(2, 'Jane', 'Smith', 'jane.smith@email.com', '9876543210', '456 Oak Avenue');
```

### Seed SalesReps table
```sql
INSERT INTO SalesReps VALUES 
(1, 'Alice', 'Johnson', 'alice.j@email.com', '1122334455'),
(2, 'Bob', 'Williams', 'bob.w@email.com', '2233445566');
```


### Seed Sales table
```sql
INSERT INTO Sales VALUES 
(1, 1, 1, 1, '2025-07-01', 24500.00),
(2, 2, 2, 2, '2025-07-15', 21500.00);
```

### Update avaliblity of vehicles
```sql
UPDATE Cars SET Availability = FALSE WHERE CarID IN (1, 2);
```

### SALES QUERY:
#### **All Sales with Full Details**
```sql
SELECT 
    S.SaleID,
    C.Make || ' ' || C.Model AS Car,
    CU.FirstName || ' ' || CU.LastName AS Customer,
    R.FirstName || ' ' || R.LastName AS SalesRep,
    S.SaleDate,
    S.SalePrice
FROM Sales S
JOIN Cars C ON S.CarID = C.CarID
JOIN Customers CU ON S.CustomerID = CU.CustomerID
JOIN SalesReps R ON S.RepID = R.RepID;
```
![[Screenshot 2025-07-24 at 11.19.19 AM.png]]
#### **Total Sales Value by Each SalesRep**
```sql
SELECT 
    R.RepID,
    R.FirstName || ' ' || R.LastName AS SalesRep,
    COUNT(S.SaleID) AS TotalSales,
    SUM(S.SalePrice) AS TotalRevenue
FROM Sales S
JOIN SalesReps R ON S.RepID = R.RepID
GROUP BY R.RepID;
```
![[Screenshot 2025-07-24 at 11.19.33 AM.png]]


### A)
```sql
SELECT DISTINCT Make FROM Cars;
```

![[Screenshot 2025-07-24 at 11.22.44 AM.png]]

### B)
```sql
SELECT * FROM Cars
WHERE Availability = TRUE
  AND Price > 25000
  AND Year >= 2022;
```
![[Screenshot 2025-07-24 at 11.23.10 AM.png]]

### C)
```sql
SELECT * FROM Cars
WHERE Price BETWEEN 20000 AND 30000;
```
![[Screenshot 2025-07-24 at 11.23.38 AM.png]]

### D)
```sql
SELECT * FROM Cars
ORDER BY Price ASC;
```
![[Screenshot 2025-07-24 at 11.23.56 AM.png]]

### E)
```sql
SELECT * FROM Cars
WHERE Price IS NULL;
```
![[Screenshot 2025-07-24 at 11.24.16 AM.png]]

### F)
```sql
SELECT * FROM Cars
ORDER BY Price DESC
LIMIT 3;
```
![[Screenshot 2025-07-24 at 11.24.33 AM.png]]

### G)
```sql
SELECT 
    MIN(Price) AS CheapestCar,
    MAX(Price) AS MostExpensiveCar,
    AVG(Price) AS AverageCarPrice,
    COUNT(CarID) AS TotalCars
FROM Cars;
```
![[Screenshot 2025-07-24 at 11.24.57 AM.png]]
