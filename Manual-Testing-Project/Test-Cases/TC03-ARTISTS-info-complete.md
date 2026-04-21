# TC03 - Koel | Artists | Artists are displayed with complete and correct information

## Preconditions
- User is registered and logged into Koel: https://qa.koel.app/#!/home  
- User is on the Artists page of the Koel app: https://qa.koel.app/#!/artists  
- Artists exist in the database

## Test Data
- Artist: Enter Value...  
- Expected metadata values: Enter Value...

## Steps
- Navigate to https://qa.koel.app/#!/artists  
- Observe the list of displayed artists  
- Review the artist name, number of albums, number of songs, and number of plays  
- Check for missing text or broken images

## Expected Result
- Artist name, number of albums, number of songs, and number of plays are visible.  
- No missing text or broken images are present.

## Actual Result
- "Unknown Artist" is displayed despite artist names being present in track data.  
- Example: https://qa.koel.app/#!/artist/1

## Status
❌ **Failed**

## Evidence
- Screenshot: TC03-1  
- Screenshot: TC03-2  
- Screenshot: 
