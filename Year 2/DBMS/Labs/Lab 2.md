___
## Introduction:

Database Management Systems (DBMS) are essential tools for organizing, storing, and retrieving data efficiently in structured form. Relational databases organize data into tables with relationships between them. In this experiment, we design a University Database with three related tables: FACULTIES, COURSES, and STUDENTS. The FACULTIES table stores details of faculty members, the COURSES table stores information about courses linked to faculties, and the STUDENTS table stores information about enrolled students. Understanding table relationships using primary and foreign keys is crucial to maintain data integrity and perform efficient queries.
# AIM:

Create a University Database with a table for FACULTIES, COURSES, STUDENTS, The attributed of the FACULTIES table should include faculty_id, first_name, last_name,department,email . The attributes of COURSES table should include course_id,course_name,faculty_id. The STUDENTS table should have attributes student_id,first_name,last_name,email,enrollment_year,course_id.
Insert Values into the Students table and showcase the student table
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
## Conclusion:

In this experiment, we successfully created a University Database with three interrelated tables: FACULTIES, COURSES, and STUDENTS. We inserted sample data into each table, verified data integrity constraints, and performed relational queries using JOINs. This helped us understand the importance of relational modeling, primary and foreign keys, and how they maintain data consistency. The experiment provides a basic foundation for designing more complex relational databases in real-world applications.