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
SELECT *
FROM student
WHERE Name LIKE "r%"
//name which is start with r, no matter what is the next character. 
//%r means no matter what is the first character, but end with r. 
or, 
SELECT *
FROM student
WHERE Name LIKE "%ar%"
//if any name contain ar then it will show in the output. 
```
```
SELECT *
FROM student
WHERE Name LIKE "_u%"
//first character is doesnot matter. if the second character is
u then the name will be print. we can also use __(double under score)
```
```
SELECT Roll as ID, Name as "First_Name"
FROM student
//for custom the table column name. 
```
```
CREATE TABLE teacher(
	ID int, 
    Name varchar(20)
);
INSERT INTO teacher(ID, Name)
VALUES
(12, "musfiq")
```
```
CREATE TABLE teacher_two(
	ID int NOT NUll AUTO_INCREMENT,
    Name varchar(20) NOT NULL,
    PRIMARY KEY(ID)
);
INSERT INTO teacher_two(ID, Name)
VALUES
(10, "Rahim"), 
(11, "Karim")
INSERT INTO teacher_two(Name)
VALUES
("Abdul") //id will auto increment. 
INSERT INTO teacher_two(ID)
VALUES
(14)
UPDATE teacher_two
SET Name="Kire"
WHERE ID=14; 

/*
UPDATE  teacher_two
SET salary = salary + 5000
WHERE salary > 10000
*/
```
```
DELETE FROM teacher_two
WHERE ID=14; 
```
```
SELECT UPPER("daffodil university");
//we can also use LOWER
```
```
SELECT UPPER(City)
FROM student
//convert uppercase of a column. 
//SELECT UPPER(City) AS Home
```
```
SELECT concat("i am", " rahim")
//concat or adding two string. 
```
```
SELECT greatest(1, 5, 3, 8, 9)
//we can also use least()
```
```
SELECT pow(2, 3)
SELECT log10(2)
SELECT TRUNCATE(12.3422354234523, 2) //for pirnting two decimal palce. 
SELECT TRUNCATE(LOG(2), 2)
SELECT rand(); 
SELECT exp(3) //which is e to the power 3
```
```
DESCRIBE student
//show the student table field and data type. 
```
```
SELECT COUNT(*)
FROM teacher
```
```
SELECT MAX(ID)
FROM teacher
//we can also use MIN
```
```
SELECT SUM(ID), AVG(ID)
FROM teacher
```
```
SELECT MIN(GPA)
FROM student
WHERE Gender="Male"
```
```
SELECT *
FROM student
WHERE Age > (SELECT AVG(Age) FROM student); 
//we use a query inside another query. this is called sub query. 
```
```
ALTER TABLE teacher_two
ADD Age int(5)
//add a new column into a table. 
```
```
ALTER TABLE teacher_two
CHANGE Age Boyos int(5)
//for rename a column name. 
```
```
ALTER TABLE teacher_two
DROP Boyos
//for deleting a column. 
```
```
UPDATE teacher_two
SET Age=20
WHERE ID=10
//for adding a value inside a null column. 
```
```
SELECT GPA, sum(GPA)
FROM student
GROUP BY Name
ORDER BY SUM(GPA) DESC
//its a group by clause. 
```
```
TRUNCATE TABLE student;
//the column name will rename as it is. but the value after the column will be removed. 
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