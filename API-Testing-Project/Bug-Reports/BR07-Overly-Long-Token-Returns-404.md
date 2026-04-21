# Bug Report: GET /api/song/{song_id}/info with an overly long Bearer token returns 404 Not Found (Should be 401 Unauthorized)

## Summary
The API incorrectly returns **404 Not Found** when requesting song information using an **overly long Bearer token**.  
A **401 Unauthorized** response is expected for overly long authentication tokens.

## Environment
- QA Environment: Koel  
- Endpoint: `GET /api/song/{song_id}/info`  
- Authentication: Overly long Bearer token  

## Preconditions
- Valid user account exists  
- Valid song ID exists in the system  
- Postman environment configured  
- Endpoint is available  
- Overly long Bearer token is used  

## Steps to Reproduce
1. Execute a **GET** request to `/api/song/{song_id}/info` using a valid song ID  
2. Include an **overly long Bearer token** in the authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **401 Unauthorized**.  
- Response body indicates that authentication is required.  
- No song information is displayed.  

## Actual Result
- Response status: **404 Not Found**.  
- The API did not return the expected 401 Unauthorized.   

## Evidence
Screenshot: [TC07](/API-Testing-Project/Evidence/Screenshots/TC07.png)
