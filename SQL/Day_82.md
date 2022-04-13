## Learning Goal 
Convert Rows to Columns in SQL

### Problem Statement

### Steps to follow
1. Create a database
2. create a table demo_table in the database.

CREATE TABLE demo_table(
NAME varchar(30),
COLLEGE varchar(30),
EXAM_DATE DATE,
SUBJECTS varchar(30),
MARKS int); 

3. Insert data into the table
4. Convert the rows into column.

### Sample Input data
| NAME    | COLLEGE | ROLL NUMBER | SUBJECT    | MARKS |
|---------|---------|-------------|------------|-------|
| ROMY    | BVP     | 0261150     | DBMS       | 90    |
| ROMY    | BVP     | 0261150     | NETWORKING | 87    |
| ROMY    | BVP     | 0261150     | GRAPHICS   | 95    |
| PUSHKAR | MSIT    | 0898888     | DBMS       | 91    |
| PUSHKAR | MSIT    | 0898888     | NETWORKING | 90    |
| PUSHKAR | MSIT    | 0898888     | GRAPHICS   | 78    |

### Sample Output data
| NAME    | COLLEGE | ROLL NUMBER | DBMS | NETWORKING | GRAPHICS |
|---------|---------|-------------|------|------------|----------|
| ROMY    | BVP     | 0261150     | 90   | 87         | 95       |
| PUSHKAR | MSIT    | 0898888     | 91   | 90         | 78       |

### Hint
Use Pivot function
