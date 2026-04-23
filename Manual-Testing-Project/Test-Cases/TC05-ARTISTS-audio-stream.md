# TC05 - Koel | Artists | Played song returns audio stream

## Preconditions
- User is registered and logged into Koel: https://qa.koel.app/#!/home  
- At least one song exists in the application  
- API endpoint for playing a song is available  

## Test Data 
- Song ID: 06cd19b77127f1e7f889ecad54376b30  

## Steps
1. Ensure at least one song is available on https://qa.koel.app/#!/home  
2. Send a GET request to the API endpoint to play a song  
3. Include the song ID in the request  
4. Observe the response status code  
5. Validate the response body  

## Expected Result
- Response status code is 200 OK.  
- Response body matches the expected string.

## Actual Result
- Response status code is 200 OK.  
- Response body matches the expected string.

## Status
✅ **Passed**

## Evidence
- Screenshot: [TC05](/Manual-Testing-Project/Evidence/TC05.png)
