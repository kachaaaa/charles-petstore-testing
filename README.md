# Charles Proxy API Testing (Petstore)

## Project Description
This project demonstrates API testing using Charles Proxy.

The goal is to intercept, analyze, and modify HTTP requests and observe server responses.

Tested API:
https://petstore.swagger.io/

## Tools
- Charles Proxy
- REST API
- Mobile browser

## What was tested
- GET /pet/{petId}
- Request/Response structure
- Status codes
- Input validation

## Techniques used
- Traffic interception
- Breakpoints
- Request modification
- Replay

## Key findings
- API returns 404 for non-existing IDs
- API returns 405 for incorrect HTTP method
- API returns 500 for invalid ID type 
