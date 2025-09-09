___
## Introduction:

Databases are critical for organizing structured data and retrieving it efficiently. In this experiment, we create a simple **Department Database** that contains employee records in a `department_table`. The table tracks each employee’s first name, last name, designation, and date of joining. The goal is to perform SQL operations such as retrieving minimum, maximum, average, and filtered records using BETWEEN, as well as ordering results in ascending/descending order and limiting results to the top 5 records.
## Observations:

- The `MIN(Join_Date)` correctly returns the earliest date an employee joined the department.
    
- The `MAX(Join_Date)` returns the most recent employee join date.
    
- The `AVG(SNo)` provides the average serial number (auto-incremented ID).
    
- The `BETWEEN` clause successfully filters employees who joined in a specific date range.
    
- Sorting in **ascending** and **descending order** works as expected based on `Join_Date`.
    
- `LIMIT 5` returns the top 5 most recent employees in the descending order of join date.
# Question 1:

Create a Department table,
The database name should be named department_db
in that the  department_table should contain

| s.no | e first name | e last name | e designation | join date |
| ---- | ------------ | ----------- | ------------- | --------- |

## Find 
- Minimum
- Maximum
- Average
- Between
- Ascending order
- Descending order
- Top 5 

### Step 1(Create Table):
```sql
create table
  `department_table` (
    `SNo` int unsigned not null,
    `E_First_Name` VARCHAR(255) null,
    `E_Last_Name` VARCHAR(255) null,
    `E_Designation` VARCHAR(255) null,
    `Join_Date` DATE null,
    primary key (`SNo`)
  );

alter table
  `department_table`
modify column
  `SNo` int unsigned not null auto_increment
```

### Step 2(Seed Values):
```sql
INSERT INTO `department_table` (
  `E_Designation`,
  `E_First_Name`,
  `E_Last_Name`,
  `Join_Date`
)
VALUES
  ('Professor', 'John', 'Doe', '2021-08-15'),
  ('Assistant Professor', 'Jane', 'Smith', '2022-01-10'),
  ('Lecturer', 'Alice', 'Johnson', '2020-05-25'),
  ('Dean', 'Bob', 'Brown', '2019-03-30');

```

### Step 3:

#### Minimum:
```sql
SELECT MIN(`Join_Date`) AS Earliest_Join_Date
FROM `department_table`;
```
![[Screenshot 2025-07-31 at 3.05.45 PM.png]]
#### Maximum:
```sql
SELECT MAX(`Join_Date`) AS Newest_Join_Date
FROM `department_table`;
```
![[Screenshot 2025-07-31 at 3.06.25 PM.png]]
### Average:
```sql
SELECT AVG(`SNo`) AS Average_ID
FROM `department_table`;
```
![[Screenshot 2025-07-31 at 3.07.00 PM.png]]

#### Between
```sql
SELECT *
FROM `department_table`
WHERE `Join_Date` BETWEEN '2020-01-01' AND '2022-12-31';
```
![[Screenshot 2025-07-31 at 3.07.16 PM.png]]
#### Ascending order:
```sql
SELECT *
FROM `department_table`
ORDER BY `Join_Date` ASC;
```
![[Screenshot 2025-07-31 at 3.07.30 PM.png]]
#### Descending order:
```sql
SELECT *
FROM `department_table`
ORDER BY `Join_Date` DESC;
```
![[Screenshot 2025-07-31 at 3.07.46 PM.png]]
#### Top 5:
```sql
SELECT *
FROM `department_table`
ORDER BY `Join_Date` DESC
LIMIT 5;
```
![[Screenshot 2025-07-31 at 3.08.00 PM.png]]
## Conclusion:

We successfully created a Department Database with a single table called `department_table`. We inserted sample employee data and demonstrated important SQL queries that help retrieve and manipulate information. These operations are foundational to data analysis and reporting in relational database management. Understanding aggregate functions, filtering, ordering, and limits is essential for efficient data retrieval in practical applications.