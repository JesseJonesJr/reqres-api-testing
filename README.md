# API Testing with Postman – Reqres Simulation

## Overview

This project showcases functional API testing using [Postman](https://www.postman.com/) and the public [Reqres API](https://reqres.in). It simulates real-world API testing tasks and includes detailed test cases, assertions, and documentation.

##  Tools Used

- Postman v10+
- JavaScript (for test scripts)
- Public API: https://reqres.in

##  Endpoints Covered

| Method | Endpoint | Purpose |
|--------|----------|---------|
| GET | /api/users?page=2 | Retrieve all users |
| GET | /api/users/2 | Retrieve a single user |
| POST | /api/users | Create a new user |
| PUT | /api/users/2 | Update user information |
| POST | /api/login | Login and receive a token |

##  Project Structure

reqres-api-testing /

├── postman_collection.json # Exported Postman collection

├── api-test-cases.md # Manual test documentation

├── README.md # Project details

## Test Coverage
- ✅ Positive and negative test scenarios  
- ✅ Status code validation  
- ✅ Response body and schema validation  
- ✅ Token handling and authentication checks  

##  How to Use

1. Clone or download this repository.
2. Open Postman and import `postman_collection.json`.
3. Run each request individually to inspect response behavior and assertion results.
4. Review `api-test-cases.md` for manual documentation of each test.

---

## Disclaimer
This is an educational portfolio project and does not represent production-level testing.  
The [Reqres API](https://reqres.in) is a public demo API provided for practicing API testing.
