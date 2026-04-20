# Test Case: GET /api/song/{song_id}/info returns 200 OK

## Objective
Verifies that a valid user with a valid token can successfully retrieve song information.

## Preconditions
- Valid user account
- Valid bearer token
- Postman environment configured
- Existing song ID

## Test Data
- song_id: *(valid)*  
- token: *(valid)*  

## Steps
1. Send a GET request to `/api/song/{song_id}/info`
2. Include a valid bearer token in the authorization header
3. Submit the request
4. Observe the response

## Expected Result
- Response status: **200 OK**
- Response body contains song information fields

## Actual Result
- The request returned **200 OK.** The response body was successfully retrieved and included the expected fields: lyrics, album_info, artist_info, and youtube (some returned null values). The API behaved as expected for a valid song_id and valid token.

## Evidence
- Screenshot: [TC01](/API-Testing-Project/Evidence/Screenshots/TC01.png)
