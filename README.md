# Charles Proxy API Testing (Swagger Petstore)

## 📌 Project Description
This project demonstrates API testing using Charles Proxy.

The goal was to intercept, analyze, and modify HTTP/HTTPS requests and verify server behavior.

Tested API:
https://petstore.swagger.io/

---

##  Tools
- Charles Proxy
- REST API
- Mobile browser

---

##  What was tested
- GET /pet/{petId}
- POST /pet (data validation)
- Request and response structure
- Status codes
- Input validation

---

##  Techniques used
- Traffic interception
- Breakpoints
- Request modification (URL and body)
- Response analysis

---

##  Test scenarios
- Valid request → 200 OK
- Non-existing ID → 404 Not Found
- Invalid endpoint usage → 405 Method Not Allowed
- Invalid data type → negative testing

---

##  Key finding
- Server returns **500 Internal Server Error** when invalid ID type is provided (`"id": "abc"`)

Expected:
400 Bad Request (invalid data type)

Actual:
500 Internal Server Error

---

##  Conclusion
The API handles basic scenarios correctly but lacks proper validation for input data types, which may lead to server errors.
