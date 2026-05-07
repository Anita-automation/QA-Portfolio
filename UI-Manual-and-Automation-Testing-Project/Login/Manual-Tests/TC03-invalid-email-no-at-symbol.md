# TC03 – Invalid Email (Missing @ Symbol)

## Preconditions
- User is registered with a valid testpro.io email.
- User has a valid password for the registered account.
- User is on the Koel Login page: https://qa.koel.app/

## Test Steps
1. Enter an invalid email missing the @ symbol (e.g., testtestpro.io).
2. Enter a valid password.
3. Click the “Log in” button.

## Expected Result
- The UI displays the validation message: **“Email format is incorrect.”**
- User remains on the Login page.

## Actual Result (from execution)
- No Koel validation message is displayed.
- Browser shows native HTML5 tooltip:  
  *“Please include an '@' in the email address…”*

## Status
❌ FAIL
