# Test Case: GET /api/song/{song_id}/info with an overly long Bearer token returns 401 Unauthorized

## Objective
Verifies that the API correctly rejects requests made with an overly long Bearer token by returning **401 Unauthorized** and preventing access to song information.

## Preconditions
- Endpoint **GET /api/song/{song_id}/info** is available  
- Valid song ID exists in the system  
- Registered user credentials are available  
- Postman environment configured  
- Overly long Bearer token is used  

## Test Data
- song_id:
- token: overly long token

## Steps
1. Send a **GET** request to `/api/song/{song_id}/info` using a valid song ID  
2. Include an **overly long Bearer token** in the authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **401 Unauthorized**  
- Response body indicates that authentication is required  
- No song information is displayed  

## Actual Result
- Response status: **404 Not Found**  
- The API did not return the expected 401 Unauthorized  
- The endpoint failed to correctly validate the overly long token  

## Evidence
Screenshot: **TC04**
