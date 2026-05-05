# Bug Reports

## Bug 1: API does not validate ID type

### Description
API accepts non-numeric ID and returns 404 instead of validation error.

### Steps to Reproduce
1. Send GET request to /pet/abc

### Expected Result
400 Bad Request (invalid ID type)

### Actual Result
404 Not Found

### Severity
Medium
