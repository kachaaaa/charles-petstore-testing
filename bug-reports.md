# Bug Reports

## Bug: Server returns 500 for invalid ID type

### Description
API does not properly validate ID type and crashes when a string value is provided.

### Steps to Reproduce
1. Send POST /pet with "id": "abc"

### Expected Result
400 Bad Request 

### Actual Result
500 Internal Server Error

### Severity
Medium
