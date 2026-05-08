# TC06 – Valid Email and Incorrect Password – Automation

## Scenario
Validate that Koel displays the correct error message when the user enters a valid email but an incorrect password.

## Related Manual Test Case
- TC06-valid-email-and-incorrect-password.md

## Related Bug Report
- BR06-incorrect-password-error-not-shown.md

## Automation Logic
- Navigate to https://qa.koel.app/
- Enter valid email: anita.surewicz@testpro.io
- Enter incorrect password
- Click “Log In”
- Assert:
  - User remains on the Login page
  - (Attempted) Expected Koel validation message: "Couldn't log you in"

## Automation Result
- Confirmed: User remained on the Login page
- Not Confirmed: Expected Koel validation message

## Reason
Koel does not render a CSS‑selectable validation message for incorrect passwords.  
The login form shakes and shows a red outline, but no text message is displayed.  
Selenium cannot locate any error element.

## Evidence
- Screenshot: Login page with incorrect password entered
- Screenshot: Red outline + shake behavior
- Screenshot: IntelliJ test execution
