API Testing with Postman – Reqres Simulation

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

├── postman_collection.json

├── api-test-cases.md

├── README.md


##  How to Use

1. Clone or download this repository.
2. Open Postman and import `postman_collection.json`.
3. Run each request individually to inspect response behavior and assertion results.
4. Review `api-test-cases.md` for manual documentation of each test.

---

> This project is part of my QA engineering portfolio and represents foundational knowledge in API testing using Postman.
