# 📧 Email Microservice Tests

This repository contains test artifacts (manual and automated) for an email dispatch microservice.

---

## 📌 API Endpoint

**Endpoint:**  
`POST /send-email`

> ⚠️ **Note:** Base URL not provided – Postman tests are structured for simulation and documentation purposes only.

---

## 📤 Sample Request Payload

```json
{
  "to": "user@example.com",
  "subject": "Welcome!",
  "body": "Thanks for signing up."
}

✅ Manual Test Coverage
✅ Valid request returns 202 Accepted

❌ Missing to field returns 422 Bad Request

❌ Invalid email format returns 422 Bad Request

❌ Queue full returns 503 Service Unavailable

❌ Invalid/malformed JSON returns 400 Bad Request

Test cases are designed to ensure RESTful compliance, input validation, and error handling.

🤖 Automation
Postman collection includes the following test scenarios:

Successful email dispatch

Missing required field

Invalid email format

Simulated queue overload (documented only)

⚠️ Actual execution requires a working base URL or mock server.

📁 Files in this Repo
email-microservice.postman_collection.json: Main Postman collection

Email Dispatch Service Tests.postman_collection.json: Backup/reference copy

README.md: You're reading it!

👤 Author
Abduliman1 – QA Engineer
🔗 GitHub Profile

📄 License
This repository is for interview and demonstration purposes only.

yaml

---

