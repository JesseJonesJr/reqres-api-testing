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

##  Test Case 3: POST Create User

- **Method**: POST
- **Endpoint**: /api/users

### Description:
Creates a new user with `name` and `job` fields.

###  Request Payload:
```json
  "name": "Jesse QA",
  "job": "Automation Engineer"
```

### Assertions:

    Status code is 201

    name = "Jesse QA"

    job = "Automation Engineer"

    id and createdAt fields exist

---

##  Test Case 4: PUT Update User

- **Method**: PUT  
- **Endpoint**: /api/users/2

###  Description:
Updates an existing user's name and job.

###  Request Payload:
```json 
  "name": "Jesse QA",
  "job": "Lead QA Engineer"
```

 Assertions:

    Status code is 200

    name = "Jesse QA"

    job = "Lead QA Engineer"

    updatedAt timestamp is returned
---

## ✅ Test Case 5: POST Login

- **Method**: POST  
- **Endpoint**: /api/login

###  Description:
Logs in a user with valid credentials and returns an authentication token.

###  Request Payload:
```json
  "email": "eve.holt@reqres.in",
  "password": "cityslicka"
```

 Assertions:

    Status code is 200

    token exists and is a non-empty string

    Response time is under 1000ms
