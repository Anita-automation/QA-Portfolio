# TC06 – Valid Email and Incorrect Password

## Preconditions
- User is registered with a valid testpro.io email.
- User knows the correct email for the account.
- User is on the Koel Login page: https://qa.koel.app/

## Test Steps
1. Enter a valid registered email (e.g., anita.surewicz@testpro.io).
2. Enter an incorrect password.
3. Click the “Log in” button.

## Expected Result
- The UI displays the message: “Couldn't log you in.”
- User remains on the Login page.

## Actual Result (from execution)
- No “Couldn't log you in” message is displayed.
- The login form briefly shakes and shows a red outline.
- No text feedback is provided.
- User remains on the Login page.

## Status
❌ FAIL

## Evidence

- Screenshot: [TC06 – IntelliJ Execution Result](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_IntelliJ-invalidPasswordShown.png)
- Screenshot: [TC06 – IntelliJ Login Attempt (Valid Email + Invalid Password)](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_IntelliJ-loginValidEmailInvalidPassword.png)
- Screenshot: [TC06 – UI Error State](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_UI.png)
