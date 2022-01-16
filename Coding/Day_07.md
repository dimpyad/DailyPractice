## Problem 1
#### Topic: Arrays, List, String
#### Difficulty Level: Easy
You are the receptionist at a hotel which has 10 floors, numbered from 0 to 9 and each floor has 26 rooms named from ‘A’ to ‘Z’. Being a receptionist your task is to handle booking queries.
You get booking queries in the form of strings of size 3 where 1st character is ‘+’ means room is booked, or ‘-’ means room is freed. Second character represents the floor of the room i.e, ‘0’ to ‘9’. Third character represents the room name i.e, ‘A’ to ‘Z’.
On booking of each room you collect 1 coin from the customer. After the end of all the booking queries you have to count the number of coins you collected.
You may assume that the list describes a correct sequence of bookings in chronological order i.e., only free rooms can be booked, and only booked rooms can be freed.

### Example:
Consider booking queries to be ["+1A", "+3E", "-1A", "+4F", "+1A", "-3E"]
- +1A: Room A on the 1st floor is booked and you collected 1 coin.
- +3E: Room E on the 3rd floor is booked and you collected 1 coin.
- -1A: Room A on the 1st floor is freed.
- +4F: Room F on the 4th floor is booked and you collected 1 coin.
- +1A: Room A on the 1st floor is booked and you collected 1 coin.
- -3E: Room E on the 3rd floor is freed.So you collected 4 coins.

### Input Format:
List of strings representing booking queries.

### Output Format :
Return an integer denoting the count of coins you collected.

### Constraints:
- 0 <= N <= 6*10^2
- |query.length| = 3


### Sample Input 1:
["+1A", "+3E", "-1A", "+4F", "+1A", "-3E"]
### Sample Output 1:
4

### Sample Input 2:
["+0A", "+0B", "+0C"]
### Sample Output 2:
3

## Problem 2
### Topic: Arrays and String
### Difficulty Level: Easy
Write a function that converts HEX string to RGB string and write another fucntion to convert RGB string to HEX string. 
Note. You are not supposed to use any built in libraries.

### Sample Input string hex to rgb
f4e3d8
### Sample output string
RGB(244, 227, 216)

### Sample input RGB to hex
[231, 55, 145]
### Sample output RGB to hex
E73791
