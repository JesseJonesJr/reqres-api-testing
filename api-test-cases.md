# API Test Cases – Reqres API

This file contains manual documentation of API test cases created and executed using Postman.

---

## Test Case 1: GET All Users

- **Method**: GET
- **Endpoint**: `/api/users?page=2`

### Description:
Retrieves a paginated list of users.

###  Assertions:
- Status code is 200
- Response time is below 1000ms
- At least one user object exists in `data[]`

---

## Test Case 2: GET Single User

- **Method**: GET
- **Endpoint**: `/api/users/2`

###  Description:
Fetches details of user with ID 2.

### Assertions:
- Status code is 200
- `first_name` is `"Janet"`
- `email` is in valid format
- `avatar` field is present and non-empty

---

##  Upcoming Test Cases

- POST Create User
- PUT Update User
- POST Login (with token handling)
