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

## Traceability
- Automation Test: [TC05 Automation](/UI-Manual-and-Automation-Testing-Project/Login/Automation/TC05_EmptyEmailAndPasswordFieldsTest.md)
- Bug Report: [BR05 – Empty Fields Error Not Shown](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR05/BR05-empty-fields-error-not-shown.md)

## Evidence

## Evidence

- Screenshot: [TC06 – IntelliJ Execution Result](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_IntelliJ-invalidPasswordShown.png)
- Screenshot: [TC06 – IntelliJ Login Attempt (Valid Email + Invalid Password)](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_IntelliJ-loginValidEmailInvalidPassword.png)
- Screenshot: [TC06 – UI Error State](/UI-Manual-and-Automation-Testing-Project/Login/Bug-Reports/BR06/TC06_incorrect-password_UI.png)
