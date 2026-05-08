# TC04 – Invalid Email (Missing Dot Symbol)

## Preconditions
- User is registered with a valid testpro.io email.
- User has a valid password for the registered account.
- User is on the Koel Login page: https://qa.koel.app/

## Test Steps
1. Enter an invalid email missing the dot symbol (e.g., anitasurewicz@testpro.io).
2. Enter a valid password.
3. Click the “Log in” button.

## Expected Result
- The UI displays the message: “Email format is incorrect.”
- User remains on the Login page.

## Actual Result (from execution)
- No “Email format is incorrect” message is displayed.
- The login form briefly shakes and shows a red outline.
- No text feedback is provided.
- User remains on the Login page.

## Status
❌ FAIL
