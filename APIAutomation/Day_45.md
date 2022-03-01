## Learning Goal
Validate different Json responses with dynamic or optional fields.

### Problem Statement #1
Validate response schema with optional field. For example the following two responses email field is optional.

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
Validate response schema when nested json has optional field. For example the following scenario, state field under address is optional.

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
Validate responses when the value of a field is dynamic. For example id is dynamic and unique every time and should be a positive number.

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
