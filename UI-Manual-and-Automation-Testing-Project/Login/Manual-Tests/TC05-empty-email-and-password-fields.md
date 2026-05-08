# TC05 – Empty Email and Password Fields

## Preconditions
- User is on the Koel Login page: https://qa.koel.app/

## Test Steps
1. Leave the email field empty.
2. Leave the password field empty.
3. Click the “Log in” button.

## Expected Result
- The UI displays the message: “Email format is incorrect.”
- User remains on the Login page.

## Actual Result (from execution)
- No “Email format is incorrect” message is displayed.
- Browser shows native HTML5 tooltip:  
  “Please fill out this field”
- User remains on the Login page.

## Status
❌ FAIL
