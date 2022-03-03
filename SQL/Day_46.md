## Leanring Goal
SQL Joins

### Problem statement #1
You have following two tables:
```
CREATE TABLE `advisors` (
  `advisor_id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(255) NOT NULL,
  `last_name` varchar(255) NOT NULL,
  PRIMARY KEY (`advisor_id`)
)

CREATE TABLE `students` (
  `student_id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(255) NOT NULL,
  `last_name` varchar(255) NOT NULL,
  `advisor_id` int(11) DEFAULT NULL,
  PRIMARY KEY (`student_id`),
  KEY `advisor_id` (`advisor_id`),
  CONSTRAINT `students_ibfk_1` FOREIGN KEY (`advisor_id`) REFERENCES `advisors` (`advisor_id`)
);

```
Here is the sample data:
```
SELECT * FROM students;

+------------+------------+------------+------------+
| student_id | first_name | last_name  | advisor_id |
+------------+------------+------------+------------+
|          1 | Tanisha    | Blake      |          2 |
|          2 | Jess       | Goldsmith  |       NULL |
|          3 | Tracy      | Wu         |          3 |
|          4 | Alvin      | Grand      |          1 |
|          5 | Felix      | Zimmermann |          2 |
+------------+------------+------------+------------+
5 rows in set (0.00 sec)


SELECT * FROM advisors;

+------------+------------+-----------+
| advisor_id | first_name | last_name |
+------------+------------+-----------+
|          1 | James      | Francis   |
|          2 | Amy        | Cheng     |
|          3 | Lamar      | Alexander |
|          4 | Anita      | Woods     |
+------------+------------+-----------+
4 rows in set (0.00 sec)

```
1. Pull all the information on students and their advisors, including students who are not assigned to an advisor.
Hint - Inner Join

2. Pull all the information on students and their advisors, excluding students who are not assigned to an advisor.
Hint - Left Join

3. Pull all the students who are assigned to advisors, plus a list of advisors not assigned to students 
Hint - Right Join

### Problem statement #2
A small bakery that sells brownies, cookies, pies, and other delicious treats to customers online. It keeps records of all of its online sales in an SQL database that is automatically populated as customers place orders on its site.

In the database, it has a customers table to keep track of customer contact information, and an orders table to keep track of various orders that those customers have placed. The schema of these tables is as follows:

```
CREATE TABLE customers (
	customer_id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
	first_name VARCHAR(255) NOT NULL,
	last_name VARCHAR(255) NOT NULL,
	email VARCHAR(255) NOT NULL,
	address VARCHAR(255) DEFAULT NULL,
	city VARCHAR(255) DEFAULT NULL,
	state VARCHAR(2) DEFAULT NULL,
	zip_code VARCHAR(5) DEFAULT NULL,
);

CREATE TABLE orders (
	order_id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
	customer_id INT NOT NULL,
	order_placed_date DATE NOT NULL,
	FOREIGN KEY (customer_id) REFERENCES customers (customer_id)
);
```
It's the end of 2016, and the owner of the bakery wants to write an SQL query that finds the COUNT of orders placed in 2016 by customer e-mail address. She wants to ORDER the results by the COUNT of orders placed in 2016, descending, so that she can personally send thank-you e-mails to top customers by order volume.

Can you write a query that will help the owner of the bakery to find the COUNT of all orders placed in 2016, by customer e-mail address, sorted descending?
