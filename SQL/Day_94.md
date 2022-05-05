### Learning Goal
Date and time

## problem Statement
Return the total number of comments received for each user in the last 30 days based on a current date given.

Table name:
fb_comments_count

user_id	- int

created_at	- datetime

number_of_comments	- int

### Hint
- The current date is given therefore, we take the difference of created_at field with the current date.
- Take only the comments that fall in the 30-day window.
- Aggregate the number of comments by user_id.
