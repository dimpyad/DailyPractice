## Learning Goal
Wildcard and special operators

## References
- https://www.w3schools.com/sql/sql_like.asp
- https://www.w3schools.com/sql/sql_wildcards.asp

### Problem Statement #1 (LIKE operator and % wildcard)
Write a query to retrieve the prod_id and prod_name fields from a table named Products if the prod_name contains the string 'bean bag'. 

### Problem Statement #2 (LIKE operator and % wildcard)
Write a query to retrieve the prod_id and prod_name fields from a table named Products if the prod_name start with 'Fish food' and ends with 'Local'. 

### Problem Statement #3  (LIKE operator and % wildcar and _ wildcard)
Select the column prod_name from the Products table where prod_name begins with any number of occurences of any character, followed by 'bean b', followed by a single instance of any character, followed by 'g', followed by any number of occurrences of any character.

### Problem Statement #4 (LIKE operator and % wildcard)
Create SELECT statements that test the following strings against the search string 'j%_uery' (first one has the query and result)

- 'jquery' 

Query - SELECT 'jquery' LIKE 'j%_uery'; 

Result - 1

- ' jquery' (note the leading space)
- 'jquery ' (note the trailing space)
- 'jQuery'
- 'JoeQuery'
- 'joeQuery'
