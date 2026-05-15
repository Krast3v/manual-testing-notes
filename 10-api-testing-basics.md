# Topic 10 — API Testing Basics

## What is an API

API (Application Programming Interface) — the way two systems communicate. When you click "Login", the browser sends a request to the server — that's an API call.

---

## HTTP Methods

| Method | Action | Example |
|---|---|---|
| **GET** | Retrieve data | Load my profile |
| **POST** | Create something new | Register an account |
| **PUT** | Replace the entire object | Update full profile |
| **PATCH** | Update one field only | Change only the email |
| **DELETE** | Delete | Delete the account |

---

## HTTP Status Codes

| Code | Meaning |
|---|---|
| **200** | OK — success |
| **201** | Created — object was created |
| **400** | Bad Request — error in the request |
| **401** | Unauthorized — not logged in |
| **403** | Forbidden — logged in but no permission |
| **404** | Not Found — does not exist |
| **500** | Internal Server Error — server-side error |

---

## What QA Tests in an API

- **Status code** — is the correct code returned?
- **Response body** — is the data correct?
- **Response time** — is the response fast enough?
- **Error handling** — are error messages correct for invalid input?
- **Authorization** — is a request without a token rejected with 401?

---

## Tools

- **Postman** — manual API testing (GUI)
- **RestSharp** — automated API testing in C#

---

## Interview Q&A

**Q: What is the difference between GET and POST?**
A: GET retrieves data without modifying anything — it's read-only. POST sends data to create a new resource on the server.

**Q: What does a 401 status code mean and how is it different from 403?**
A: 401 means the user is not authenticated — they haven't logged in. 403 means the user is authenticated but doesn't have permission to access that resource.

**Q: What do you check when testing an API endpoint?**
A: Status code, response body correctness, response time, error handling for invalid input, and that unauthorized requests are properly rejected.
