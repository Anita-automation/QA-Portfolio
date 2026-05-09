# TC04 – Invalid Email (Missing Dot Symbol) – Automation

## Scenario
Validate that Koel displays the correct error message when the user enters an email address missing the dot symbol.

## Related Manual Test Case
- TC04-invalid-email-no-dot-symbol.md

## Related Bug Report
- BR04-missing-dot-symbol-expected-error-message-not-shown.md

## Automation Logic
- Navigate to https://qa.koel.app/
- Enter invalid email: anitasurewicz@testpro.io
- Enter valid password
- Click “Log In”
- Assert:
  - User remains on the Login page
  - (Attempted) Expected Koel validation message: "Email format is incorrect"

## Automation Result
- Confirmed: User remained on the Login page
- Not Confirmed: Expected Koel validation message

## Reason
Koel does not render a CSS‑selectable validation message for this error state.  
The login form shakes and shows a red outline, but no text message is displayed.  
Selenium cannot locate any error element.

## Evidence
- Screenshot: Login page with invalid email entered
- Screenshot: Browser behavior (shake + red outline)
- Screenshot: IntelliJ test execution
