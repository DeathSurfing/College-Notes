___
```sql
USE UNIVERSITYDB;

-- Create FACULTIES
CREATE TABLE FACULTIES (
    faculty_id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    department VARCHAR(100),
    email VARCHAR(100) UNIQUE
);

-- Create COURSES
CREATE TABLE COURSES (
    course_id INT PRIMARY KEY AUTO_INCREMENT,
    course_name VARCHAR(100),
    credits INT,
    faculty_id INT,
    FOREIGN KEY (faculty_id) REFERENCES FACULTIES(faculty_id)
);

-- Create STUDENTS
CREATE TABLE STUDENTS (
    student_id INT PRIMARY KEY AUTO_INCREMENT,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    email VARCHAR(100) UNIQUE,
    enrollment_year INT,
    course_id INT,
    FOREIGN KEY (course_id) REFERENCES COURSES(course_id)
);
```


## Example insert:

```sql
INSERT INTO `UNIVERSITY_DB`.`STUDENTS`
(`student_id`,
`first_name`,
`last_name`,
`email`,
`enrollment_year`)
VALUES
(2084,
"Venella",
"Linga",
"venellalinga@woxsen.edu.in",
2024);

```


```sql
SELECT * FROM STUDENTS;
```
Returns
![[Screenshot 2025-07-24 at 10.18.48 AM.png]]
