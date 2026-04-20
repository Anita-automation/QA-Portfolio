# Test Case: GET /api/song/{song_id}/info with missing song ID returns 400 Bad Request

## Objective
Verifies that the API returns **400 Bad Request** when the user attempts to retrieve song information without providing a song ID.

## Preconditions
- Valid user account  
- Valid bearer token  
- Postman environment configured  
- Endpoint `GET /api/song/{song_id}/info` is available  

## Test Data
- song_id: *(missing)*  
- token:  

## Steps
1. Send a GET request to `/api/song//info` (omit the song ID)  
2. Include a valid bearer token in the Authorization header  
3. Submit the request  
4. Observe the response  

## Expected Result
- Response status: **400 Bad Request**  
- Response body contains an error message indicating that the song ID is missing  
- No song information is displayed  

## Actual Result
The request returned **400 Bad Request**. The response body included an error message stating that the song ID was required and not provided. No song information was displayed.

## Evidence
Screenshot: TC03
Related Bug Report: [BR03](../bug-reports/BR03_missing_song_id.md)
