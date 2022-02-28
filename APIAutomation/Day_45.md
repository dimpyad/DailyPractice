## Learning Goal
Validate different Json responses with dynamic or optional data.

### Problem Statement #1
Validate the following two responses when field email is optional.

Response 1:
```
{
  "id": 1,
  "first_name": "Test",
  "last_name": "1",
  "phone": 123456,
  "email": "test1@gmail.com"
}
```
Response 2:
```
{
  "id": 2,
  "first_name": "Test",
  "last_name": "2",
  "phone": 5446456,
}
```
### Problem Statement #2
Validate the following two responses when field state is optional in the nested json with key address.

Response 1:
```
{
  "id": 1,
  "first_name": "Test",
  "last_name": "1",
  "address":
  {
    "address line 1": "test",
    "city": "Bangalore",
    "state": "Karnataka"
  }
}
```
Response 2:
```
{
  "id": 2,
  "first_name": "Test",
  "last_name": "2",
  "address":
  {
    "address line 1": "test",
    "city": "Chennai",
  }
}
```
### Problem Statement #3
Validate the following two responses when the value of a field is dynamic for example id is dynamic and unique every time and should be an positive number.
Response 1:
```
{
  "id": 1,
  "first_name": "Test",
}
```
Response 2:
```
{
  "id": 2,
  "first_name": "Test",
}
```
