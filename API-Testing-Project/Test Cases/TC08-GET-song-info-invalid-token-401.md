# Test Case: GET /api/song/{song_id}/info with an invalid Bearer token returns 401 Unauthorized

## Objective
Verifies that the API correctly rejects requests made with an invalid Bearer token by returning **401 Unauthorized** and preventing access to song information.

## Preconditions
- Endpoint **GET /api/song/{song_id}/info** is available  
- Valid song ID exists in the system  
- Registered user credentials are available  
- Postman environment configured  
- Invalid Bearer token is used  

## Test Data
- song_id: *(valid)*
- token: *(invalid token)*

## Steps
1. Send a **GET** request to `/api/song/{song_id}/info` using a valid song ID  
2. Include an **invalid Bearer token** in the authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **401 Unauthorized**  
- Response body indicates that authentication is required  
- No song information is displayed  

## Actual Result
- Response status: **200 OK**    
- This behavior violates expected authentication

## Evidence
- Screenshot: [TC08](/API-Testing-Project/Evidence/Screenshots/TC08.png)
- Related Bug Report: [BR08-Invalid-Token-Returns-200.md](../Bug-Reports/BR08-Invalid-Token-Returns-200.md)
