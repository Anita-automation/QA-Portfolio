# Test Case: GET /api/song/{song_id}/info with missing song ID returns 404 Not Found

## Objective
Verifies that the API returns **404 Not Found** when the user attempts to retrieve song information without providing a song ID, resulting in an invalid route.

## Preconditions
- Valid user account  
- Valid bearer token  
- Postman environment configured  
- Endpoint `GET /api/song/{song_id}/info` is available  

## Test Data
- song_id: *(missing)*  
- token  

## Steps
1. Send a GET request to `/api/song//info` (omit the song ID)  
2. Include a valid bearer token in the authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **404 Not Found**  
- Response body indicates that the route or resource was not found  
- No song information is displayed  

## Actual Result
- The request returned **404 Not Found**.  
- The response body contained an empty `"message"` field.  
- No song information was displayed.  

## Evidence
- Screenshot: TC03
