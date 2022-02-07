You have two SQL tables. The first one is called employees and it contains the employee names, the unique employee ids and the department names of a company. 

Example:
| department_name | employee_id | employee_name     |  
|-----------------|-------------|-------------------|
| Sales           | 123         | John Doe          |  
| Sales           | 211         | Jane Smith        |  
| HR              | 556         | Billy Bob         |  
| Sales           | 711         | Robert Hayek      |  
| Marketing       | 235         | Edward Jorgson    |   
| Marketing       | 236         | Christine Packard |  

The second table is named salaries. It holds the same employee names and the same employee ids and the salaries for each employee. 
Example:
| salary | employee_id | employee_name     |
|--------|-------------|-------------------|
| 500    | 123         | John Doe          |
| 600    | 211         | Jane Smith        |
| 1000   | 556         | Billy Bob         |
| 400    | 711         | Robert Hayek      |
| 1200   | 235         | Edward Jorgson    |
| 200    | 236         | Christine Packard |

Write a query to get every department where the average salary per employee is lower than $500.
