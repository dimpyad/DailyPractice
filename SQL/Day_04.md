### Problem 1
```
SELECT column, AGG_FUNC(column_or_expression), …
  FROM a_table
 INNER JOIN some_table
       ON a_table.column = some_table.column
 WHERE a_condition
 GROUP BY column
HAVING some_condition
 ORDER BY column
 LIMIT 5;
```
In what order does SQL run the clauses? Select the correct option from the list of choices below:
1. SELECT, FROM, WHERE, GROUP BY
2. FROM, WHERE, HAVING, SELECT, LIMIT
3. SELECT, FROM, INNER JOIN, GROUP BY
4. FROM, SELECT, LIMIT, WHERE

### Problem 2
Given the table below, write a SQL query that retrieves the personal data about alumni who scored above 16 on their calculus exam.

alumni
| student_id | name    | surname | birth_date | faculty        |
|------------|---------|---------|------------|----------------|
| 347        | Daniela | Lopes   | 1991-04-26 | Medical School |
| 348        | Robert  | Fischer | 1991-03-09 | Mathematics    |

evaluation
| student_id | class_id | exam_date  | grade |
|------------|----------|------------|-------|
| 347        | 74       | 2015-06-19 | 16    |
| 347        | 87       | 2015-06-06 | 20    |
| 348        | 74       | 2015-06-19 | 13    | 

curriculum
| class_id | class_name | professor_id | semester    |
|----------|------------|--------------|-------------|
| 74       | algebra    | 435          | 2015_summer |
| 87       | calculus   | 532          | 2015_summer |
| 46       | statistics | 625          | 2015_winter |
