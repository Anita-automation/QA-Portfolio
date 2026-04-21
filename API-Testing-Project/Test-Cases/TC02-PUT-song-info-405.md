# Test Case: PUT /api/song/{song_id}/info returns 405 Method Not Allowed

## Objective
Verifies that the API correctly rejects unsupported HTTP methods by returning **405 Method Not Allowed** when a user attempts to update song information using the PUT method.

## Preconditions
- Valid user account  
- Valid Bearer token  
- Postman environment configured  
- Existing song ID  
- Endpoint **GET /api/song/{song_id}/info** is available  

## Test Data
- song_id: *(valid)*  
- token: *(valid)*  

## Steps
1. Send a **PUT** request to `/api/song/{song_id}/info`  
2. Include a valid Bearer token in the Authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **405 Method Not Allowed**.  
- Response body contains an error message indicating that the **PUT** method is not supported and only **GET, HEAD** are allowed.  

## Actual Result
- The request returned **405 Method Not Allowed**.  
- The response body included an error message stating that the **PUT** method is not supported for this route and that only **GET** and **HEAD** are allowed.  
- The API behaved as expected when an unsupported HTTP method was used with a valid song ID and valid token.

## Evidence
- Screenshot: [TC02](/API-Testing-Project/Evidence/Screenshots/TC02.png)
