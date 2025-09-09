___
# MySQL Advanced Query Operators - DBMS LAB 7

## Database Schema Setup

First, create the database and Students table with sample data:

```sql
-- Create the database
CREATE DATABASE dbms_lab7;
USE dbms_lab7;

-- Create Students table
CREATE TABLE Students (
    ID INT PRIMARY KEY,
    Name VARCHAR(100) NOT NULL,
    Course VARCHAR(50) NOT NULL,
    DOB DATE NOT NULL,
    Gender CHAR(1) NOT NULL
);

-- Insert sample data
INSERT INTO Students (ID, Name, Course, DOB, Gender) VALUES
    (1, 'Alice Johnson', 'CSE-AIML', '2003-05-15', 'F'),
    (2, 'Bob Smith', 'CSE-AIML', '2002-08-22', 'M'),
    (3, 'Charlie Brown', 'CSE', '2003-01-10', 'M'),
    (4, 'Diana Prince', 'CSE-AIML', '2002-12-05', 'F'),
    (5, 'Edward Davis', 'ECE', '2003-03-18', 'M'),
    (6, 'Fiona Green', 'CSE', '2002-11-30', 'F'),
    (7, 'George Wilson', 'ECE', '2003-07-08', 'M'),
    (8, 'Hannah Lee', 'CSE-AIML', '2002-09-14', 'F'),
    (9, 'Ian Miller', 'CSE', '2003-04-25', 'M'),
    (10, 'Anna Taylor', 'CSE-AIML', '2002-06-12', 'F');
```
![[Screenshot 2025-09-04 at 11.49.25 AM.png]]
## Initial Data Verification

```sql
-- View all students data
SELECT * FROM Students ORDER BY ID;

-- Quick overview of data distribution
SELECT 
    Course, 
    COUNT(*) AS Total_Students,
    COUNT(CASE WHEN Gender = 'M' THEN 1 END) AS Male_Count,
    COUNT(CASE WHEN Gender = 'F' THEN 1 END) AS Female_Count
FROM Students 
GROUP BY Course;
```
![[Screenshot 2025-09-04 at 11.49.38 AM.png]]
## Advanced Query Operations

### 1. LIKE Operator

The LIKE operator is used for pattern matching in string data.

```sql
-- Find all students whose names start with 'A'
SELECT *
FROM Students
WHERE Name LIKE 'A%';
```
![[Screenshot 2025-09-04 at 11.49.51 AM.png]]
**Additional LIKE Examples:**

```sql
-- Names ending with 'son'
SELECT * FROM Students WHERE Name LIKE '%son';

-- Names containing 'an' anywhere
SELECT * FROM Students WHERE Name LIKE '%an%';

-- Names with exactly 3 characters starting with 'B'
SELECT * FROM Students WHERE Name LIKE 'B__';

-- Names starting with vowels
SELECT * FROM Students WHERE Name LIKE 'A%' OR Name LIKE 'E%' OR Name LIKE 'I%' OR Name LIKE 'O%' OR Name LIKE 'U%';
```
![[Screenshot 2025-09-04 at 11.50.06 AM.png]]
### 2. GROUP BY Clause

The GROUP BY clause groups rows that have the same values in specified columns.

```sql
-- Count students in each course
SELECT Course, COUNT(*) AS StudentCount
FROM Students
GROUP BY Course;
```
![[Screenshot 2025-09-04 at 11.50.23 AM.png]]
**Additional GROUP BY Examples:**

```sql
-- Group by gender and show average age (approximate)
SELECT 
    Gender,
    COUNT(*) AS StudentCount,
    AVG(YEAR(CURDATE()) - YEAR(DOB)) AS AvgAge
FROM Students 
GROUP BY Gender;

-- Group by course and gender
SELECT 
    Course,
    Gender,
    COUNT(*) AS StudentCount
FROM Students 
GROUP BY Course, Gender
ORDER BY Course, Gender;
```
![[Screenshot 2025-09-04 at 11.50.35 AM.png]]
### 3. HAVING Clause

The HAVING clause is used to filter groups created by GROUP BY.

```sql
-- Show courses with more than 2 students
SELECT Course, COUNT(*) AS StudentCount
FROM Students
GROUP BY Course
HAVING COUNT(*) > 2;
```
![[Screenshot 2025-09-04 at 11.50.49 AM.png]]
**Additional HAVING Examples:**

```sql
-- Courses with more than 1 female student
SELECT 
    Course, 
    COUNT(*) AS FemaleCount
FROM Students 
WHERE Gender = 'F'
GROUP BY Course
HAVING COUNT(*) > 1;

-- Courses with average birth year before 2003
SELECT 
    Course,
    COUNT(*) AS StudentCount,
    AVG(YEAR(DOB)) AS AvgBirthYear
FROM Students
GROUP BY Course
HAVING AVG(YEAR(DOB)) < 2003;
```
![[Screenshot 2025-09-04 at 11.50.59 AM.png]]
### 4. EXISTS Operator

The EXISTS operator tests for the existence of rows in a subquery.

```sql
-- Find all CSE-AIML students (using EXISTS to check if CSE-AIML course exists)
SELECT * FROM Students s1
WHERE EXISTS (
    SELECT 1 FROM Students s2 WHERE s2.Course = 'CSE-AIML'
)
AND s1.Course = 'CSE-AIML';
```
![[Screenshot 2025-09-04 at 11.51.25 AM.png]]
**Additional EXISTS Examples:**

```sql
-- Find students who are in the same course as student with ID 1
SELECT * FROM Students s1
WHERE EXISTS (
    SELECT 1 FROM Students s2 
    WHERE s2.ID = 1 AND s2.Course = s1.Course
) AND s1.ID != 1;

-- Find students whose course has at least one male student
SELECT * FROM Students s1
WHERE EXISTS (
    SELECT 1 FROM Students s2 
    WHERE s2.Course = s1.Course AND s2.Gender = 'M'
);
```
![[Screenshot 2025-09-04 at 11.51.59 AM.png]]
### 5. ANY Operator

The ANY operator returns true if any of the subquery values meet the condition.

```sql
-- Find students with ID greater than any CSE-AIML student's ID
SELECT *
FROM Students
WHERE ID > ANY (
    SELECT ID FROM Students WHERE Course = 'CSE-AIML'
);
```
![[Screenshot 2025-09-04 at 11.52.17 AM.png]]
**Additional ANY Examples:**

```sql
-- Students born after any male student
SELECT *
FROM Students
WHERE DOB > ANY (
    SELECT DOB FROM Students WHERE Gender = 'M'
);

-- Students with ID greater than any student in CSE course
SELECT *
FROM Students
WHERE ID > ANY (
    SELECT ID FROM Students WHERE Course = 'CSE'
);
```
![[Screenshot 2025-09-04 at 11.52.39 AM.png]]
### 6. ALL Operator

The ALL operator returns true only if all subquery values meet the condition.

```sql
-- Find students born before all male students
SELECT *
FROM Students
WHERE DOB < ALL (
    SELECT DOB FROM Students WHERE Gender = 'M'
);
```
![[Screenshot 2025-09-04 at 11.52.49 AM.png]]
**Additional ALL Examples:**

```sql
-- Students with ID greater than all CSE students
SELECT *
FROM Students
WHERE ID > ALL (
    SELECT ID FROM Students WHERE Course = 'CSE'
);

-- Students born after all students in ECE course
SELECT *
FROM Students
WHERE DOB > ALL (
    SELECT DOB FROM Students WHERE Course = 'ECE'
);
```
![[Screenshot 2025-09-04 at 11.53.07 AM.png]]
## Combined Query Examples

### Complex Queries Using Multiple Operators

```sql
-- Students whose names start with vowels and are in courses with more than 2 students
SELECT s.*
FROM Students s
WHERE s.Name LIKE 'A%' OR s.Name LIKE 'E%' OR s.Name LIKE 'I%' OR s.Name LIKE 'O%' OR s.Name LIKE 'U%'
AND EXISTS (
    SELECT 1 
    FROM Students s2 
    WHERE s2.Course = s.Course 
    GROUP BY s2.Course 
    HAVING COUNT(*) > 2
);

-- Students in courses where the average ID is greater than any ECE student's ID
SELECT *
FROM Students s1
WHERE s1.Course IN (
    SELECT Course
    FROM Students
    GROUP BY Course
    HAVING AVG(ID) > ANY (
        SELECT ID FROM Students WHERE Course = 'ECE'
    )
);
```
![[Screenshot 2025-09-04 at 11.53.29 AM.png]]
## Output Verification Queries

### 1. LIKE Output

```sql
SELECT 'LIKE OPERATOR RESULTS:' AS Operation;
SELECT * FROM Students WHERE Name LIKE 'A%';
```
![[Screenshot 2025-09-04 at 11.53.47 AM.png]]
### 2. GROUP BY Output

```sql
SELECT 'GROUP BY RESULTS:' AS Operation;
SELECT Course, COUNT(*) AS StudentCount FROM Students GROUP BY Course;
```
![[Screenshot 2025-09-04 at 11.54.00 AM.png]]
### 3. HAVING Output

```sql
SELECT 'HAVING RESULTS:' AS Operation;
SELECT Course, COUNT(*) AS StudentCount FROM Students GROUP BY Course HAVING COUNT(*) > 2;
```
![[Screenshot 2025-09-04 at 11.54.21 AM.png]]
### 4. EXISTS Output

```sql
SELECT 'EXISTS RESULTS:' AS Operation;
SELECT * FROM Students s1
WHERE EXISTS (SELECT 1 FROM Students s2 WHERE s2.Course = 'CSE-AIML')
AND s1.Course = 'CSE-AIML';
```
![[Screenshot 2025-09-04 at 11.54.32 AM.png]]
### 5. ANY Output

```sql
SELECT 'ANY RESULTS:' AS Operation;
SELECT * FROM Students WHERE ID > ANY (SELECT ID FROM Students WHERE Course = 'CSE-AIML');
```
![[Screenshot 2025-09-04 at 11.54.40 AM.png]]
### 6. ALL Output

```sql
SELECT 'ALL RESULTS:' AS Operation;
SELECT * FROM Students WHERE DOB < ALL (SELECT DOB FROM Students WHERE Gender = 'M');
```
![[Screenshot 2025-09-04 at 11.54.50 AM.png]]
## Summary of Operations

| Operator     | Purpose                                 | Example Use Case                             |
| ------------ | --------------------------------------- | -------------------------------------------- |
| **LIKE**     | Pattern matching in strings             | Finding names starting with specific letters |
| **GROUP BY** | Grouping rows with same values          | Counting students per course                 |
| **HAVING**   | Filtering grouped results               | Finding courses with more than X students    |
| **EXISTS**   | Testing if subquery returns any rows    | Finding students in courses that exist       |
| **ANY**      | Comparing with any value from subquery  | Finding values greater than any in a set     |
| **ALL**      | Comparing with all values from subquery | Finding values greater than all in a set     |

Each operator serves a specific purpose in data querying and can be combined for complex data retrieval operations.