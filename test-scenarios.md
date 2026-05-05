# Test Scenarios

## Scenario 1: Get pet by valid ID
Request: GET /pet/1  
Expected: 200 OK  
Result: Passed  

---

## Scenario 2: Get pet by non-existing ID
Request: GET /pet/99999  
Expected: 404 Not Found  
Result: Passed  

---

## Scenario 3: Get pet without ID
Request: GET /pet/  
Expected: 405 Method Not Allowed  
Result: Passed  

---

## Scenario 4: Get pet with invalid ID type
Request: GET /pet/abc  
Expected: 400 Bad Request  
Actual: 404 Not Found  
Result: Failed (potential issue)
