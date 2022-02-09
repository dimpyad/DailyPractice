## Problem Statement

You have the users tables with following columns:

| user_id | username    |
|---------|-------------|
| 1       | John Doe    |
| 2       | Jane Don    |
| 3       | Alice Jones |
| 4       | Lisa Romero |

training_details table having following columns:

| user_training_id | user_id | training_id | training_date |
|------------------|---------|-------------|---------------|
| 1                | 1       | 1           | "2015-08-02"  |
| 2                | 2       | 1           | "2015-08-03"  |
| 3                | 3       | 2           | "2015-08-02"  |
| 4                | 4       | 2           | "2015-08-04"  |
| 5                | 2       | 2           | "2015-08-03"  |
| 6                | 1       | 1           | "2015-08-02"  |
| 7                | 3       | 2           | "2015-08-04"  |
| 8                | 4       | 3           | "2015-08-03"  |
| 9                | 1       | 4           | "2015-08-03"  |
| 10               | 3       | 1           | "2015-08-02"  |
| 11               | 4       | 2           | "2015-08-04"  |
| 12               | 3       | 2           | "2015-08-02"  |
| 13               | 1       | 1           | "2015-08-02"  |
| 14               | 4       | 3           | "2015-08-03"  |

Write a query to to get the list of users who took the a training lesson more than once in the same day, grouped by user and training lesson, each ordered from the most recent lesson date to oldest date.
