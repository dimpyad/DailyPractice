## Problem Statement
Consider an orders table with the following structure:

| OrderID | OrderDate  | OrderPrice | OrderQuantity | CustomerName |
|---------|------------|------------|---------------|--------------|
| 1       | 12/22/2005 | 160        | 2             | Smith        |
| 2       | 08/10/2005 | 190        | 2             | Johnson      |
| 3       | 07/13/2005 | 500        | 5             | Baldwin      |
| 4       | 07/15/2005 | 420        | 2             | Smith        |
| 5       | 12/22/2005 | 1000       | 4             | Wood         |
| 6       | 10/2/2005  | 820        | 4             | Smith        |
| 7       | 11/03/2005 | 2000       | 2             | Baldwin      |

Write query to solve the following:

1. What is the count of total no of orders?
2. What is the count of the number of orders made by a customer with CustomerName - Smith?
3. What is the total value of all the orders?
4. What is the average number of items per order? 
5. What is the average order price when the price is more than 200 and order month is July, 2005?
6. What is the minimum price paid for any of the orders?
7. What is the minimum price paid for any of the orders when orderQuantiy = 4? 
8. What is the maximum price paid for any of the orders?
9. What is the maximum price paid for any of the orders when order id > 3?
10. What is the maximum price paid for any of the orders when order month is between May and Sep?
