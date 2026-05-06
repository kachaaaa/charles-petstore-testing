Bug: Server returns 500 for invalid ID type

Description:
API does not validate ID data type and crashes when a string value is provided instead of a number.

Steps to Reproduce:
1. Send POST request to /pet with body:
   "id": "abc"

Expected Result:
400 Bad Request (invalid data type)

Actual Result:
500 Internal Server Error

Severity:
High
