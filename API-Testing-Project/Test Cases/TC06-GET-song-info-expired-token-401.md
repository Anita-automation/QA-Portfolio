# Test Case: GET /api/song/{song_id}/info with an expired Bearer token returns 401 Unauthorized

## Objective
Verifies that the API correctly rejects requests made with an expired Bearer token by returning **401 Unauthorized** and not exposing any song information.

## Preconditions
- Endpoint **GET /api/song/{song_id}/info** is available  
- Valid song ID exists in the system  
- Registered user credentials are available  
- Postman environment configured  
- Expired Bearer token is used  

## Test Data
- song_id: (valid)
- token: (expired token)

## Steps
1. Send a **GET** request to `/api/song/{song_id}/info`  
2. Include an **expired** Bearer token in the Authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **401 Unauthorized**  
- No song information is displayed  

## Actual Result
The request returned **200 OK** instead of 401 Unauthorized.  
The response body displayed HTML content rather than an authorization error.  
The API did **not** correctly reject the expired token, and the endpoint failed to enforce authentication requirements.

## Evidence
Screenshot: **TC03**  
Bug Report: 
