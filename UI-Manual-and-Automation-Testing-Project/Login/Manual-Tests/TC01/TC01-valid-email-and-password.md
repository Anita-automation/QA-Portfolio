
# TC01 – Valid Email and Password

## Preconditions
- User is registered with a valid testpro.io email.
- User has a valid password for the registered account.
- User is on the Koel Login page: https://qa.koel.app/

## Test Steps
1. Enter a valid registered email (e.g., anita.surewicz@testpro.io).
2. Enter the correct password.
3. Click the “Log in” button.

## Expected Result
- User is successfully logged in.
- User is redirected to the Homepage.

## Actual Result (from execution)
- User successfully logged in.
- User was redirected to the Homepage.

## Status
🟢 PASS

## Traceability
- Automation Test:  
  [TC01 Automation](/UI-Manual-and-Automation-Testing-Project/Login/Automation/TC01/TC01_ValidLoginTest.md)

## Evidence
- [UI Before Login](ca://s?q=Open_TC01_valid-email-password_UI-before)
- [UI After Login](ca://s?q=Open_TC01_valid-email-password_UI-after)
- [IntelliJ – Passed](ca://s?q=Open_TC01_valid-email-password_IntelliJ-Passed)
