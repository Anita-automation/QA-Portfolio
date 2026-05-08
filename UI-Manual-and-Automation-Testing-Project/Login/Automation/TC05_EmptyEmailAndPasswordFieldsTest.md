# TC05 – Empty Email and Password Fields – Automation

## Scenario
Validate that Koel displays the correct error message when both the email and password fields are left empty.

## Related Manual Test Case
- TC05-empty-email-and-password-fields.md

## Related Bug Report
- BR05-empty-fields-error-not-shown.md

## Automation Logic
- Navigate to https://qa.koel.app/
- Leave the email field empty
- Leave the password field empty
- Click “Log In”
- Assert:
  - User remains on the Login page
  - (Attempted) Expected Koel validation message: "Email format is incorrect"

## Automation Result
- Confirmed: User remained on the Login page
- Not Confirmed: Expected Koel validation message

## Reason
Koel does not render a CSS‑selectable validation message for empty fields.  
Instead, the browser displays a native HTML5 tooltip (“Please fill out this field”), which Selenium cannot capture as a DOM element.

## Evidence
- Screenshot: Browser tooltip displayed
- Screenshot: Login page with empty fields
- Screenshot: IntelliJ test execution
