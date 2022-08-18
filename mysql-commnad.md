```
show databases; 
//For showing the existing database. 
```
```
CREATE DATABASE college; 
//For creating a new database. 
```
```
DROP DATABASE college; 
//For delete a existing database. 
```
```
CREATE TABLE student(
	Roll int, 
    Name varchar(20), 
    Gender varchar(15), 
    Age int(5),
    GPA double(3, 2), 
    City varchar(20), 
    PRIMARY KEY(Roll)
);
//For creating a new table. 
```
```
RENAME TABLE student TO student_details
//For renaming a table. 
```
```
DROP TABLE student_details; 
//For delete a table completely. 
```
```
INSERT INTO student
VALUES
(01, "Rahim", "Male", 20, 3.55, "Dhaka"), 
(02, "Karim", "Male", 21, 3.56, "Cumilla"),
(03, "Abdul", "Male", 22, 3.57, "Barisha"), 
(04, "Munna", "Male", 23, 3.58, "Dhaka"), 
(05, "Siam", "Male", 24, 3.59, "Dhaka"), 
(06, "Rabbi", "Male", 25, 3.61, "Rajshahi"), 
(07, "Emon", "Male", 26, 3.62, "Pabna"), 
(08, "Abraz", "Male", 27, 3.63, "Dhaka")
//Insert info into ithe table. 
```
```
DDL: CREATE, ALTER, DROP
DML: INSERT, DELETE, UPDATE, SELECT
```
```
SELECT Roll, Name
FROM student
//select column_name from student table. 
```
```
SELECT DISTINCT City
FROM student
//distinct doesn't allow duplicate value. Its remove the duplicate value. 
```
```
SELECT *
FROM student
LIMIT 5
//for limit 5 it will show only the five row. 
```
```
SELECT *
FROM student
LIMIT 2, 5
//for limit 2, 5 it will remove the first two row then show the 5 row. 
```
```
SELECT Name, Age
FROM student
ORDER BY Name
//by default it will sort ascending order. 
```
```
SELECT Name, Age
FROM student
ORDER BY Name DESC
//for descending order we need to write desc. 
```
```
SELECT 5 + 2
//for adding two number. we can also do: -, *, /, %
```
```
SELECT DISTINCT City
FROM student
WHERE Gender="Male"
ORDER BY City; 
or, 
SELECT *
FROM student
WHERE Age > 22
//display the output based on a condition. 
```
```
SELECT Roll, Name
FROM student
WHERE Roll BETWEEN 2 AND 7
//show roll between 2 and 7
or, 
SELECT Roll, Name
FROM student
WHERE Roll != 3
//display all roll except 3
```
```
SELECT *
FROM student
WHERE Gender="Male" OR GPA > 3.6
```
```
SELECT *
FROM student
WHERE Gender="Male" AND (GPA > 3.6 OR City="Dhaka")
```
```
SELECT *
FROM student
WHERE City IN ("Dhaka", "Cumilla"); 
//find the city which name is dhaka and cumilla. we can also use NOT IN. 
```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```
```

```