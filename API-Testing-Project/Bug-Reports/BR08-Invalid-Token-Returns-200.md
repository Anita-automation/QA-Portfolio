# Bug Report: GET /api/song/{song_id}/info without a valid Bearer token returns 200 OK (Should be 401 Unauthorized)

## Summary
The API incorrectly returns **200 OK** when requesting song information without a valid Bearer token.  
A **401 Unauthorized** response is expected for unauthenticated or improperly authenticated requests.

## Environment
- QA Environment: Koel  
- Endpoint: `GET /api/song/{song_id}/info`  
- Authentication: Invalid or missing Bearer token  

## Preconditions
- Valid user account exists  
- Valid song ID exists in the system  
- Postman environment configured  
- Endpoint is available  

## Steps to Reproduce
1. Execute a **GET** request to `/api/song/{song_id}/info` using a valid song ID  
2. Do **not** include a valid Bearer token in the Authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **401 Unauthorized**  
- Response body indicates that authentication is required  
- No song information is displayed  

## Actual Result
- Response status: **200 OK**  
- The API returned a successful response despite the missing or invalid token  
- This behavior violates expected authentication and security requirements  

## Evidence
Screenshot: **BR08**
