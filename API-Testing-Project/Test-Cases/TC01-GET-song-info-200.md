# Test Case: GET /api/song/{song_id}/info returns 200 OK

## Objective
Verify that a registered user with a valid bearer token can successfully retrieve song information using a valid song ID.

## Preconditions
- Endpoint GET /api/song/{song_id}/info is available
- A valid song ID exists in the system
- Valid Bearer token for a registered user is available
- Postman environment is configured with {{baseURL}} and {{token}}

## Test Data
- song_id: <valid existing ID>
- token: <valid bearer token>

## Steps
1. Open Postman and select the request: GET /api/song/{song_id}/info
2. Insert a valid song ID into the request path
3. Ensure Authorization is set to Bearer Token and the token field contains a valid token ({{token}})
4. Send the request
5. Observe the response status and body

## Expected Result
- Response status: 200 OK
- Response body displays song information (e.g., lyrics, album_info, artist_info, youtube fields)
- User is able to retrieve song info successfully

## Actual Result
Test passed — response returned 200 OK and song info was displayed.

## Evidence
- Screenshot: /Evidence/screenshots/TC01.png
- Postman run: /Evidence/postman-collection.json
