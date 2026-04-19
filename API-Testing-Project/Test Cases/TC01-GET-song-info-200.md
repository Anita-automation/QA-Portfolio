# Test Case: GET /api/song/{song_id}/info returns 200 OK

## Objective
Verifies that a valid user with a valid token can successfully retrieve song information.

## Preconditions
- Valid user account
- Valid bearer token
- Postman environment configured
- Existing song ID

## Test Data
- song_id: <valid ID>
- token: <valid token>

## Steps
1. Send a GET request to /api/song/{song_id}/info
2. Include a valid bearer token in the Authorization header
3. Submit the request
4. Observe the response

## Expected Result
- Response status: **200 OK**
- Response body contains song information fields

## Actual Result
To be filled during execution.

## Evidence
- Screenshot: [TC01](/API-Testing-Project/Evidence/Screenshots/TC01.png)
