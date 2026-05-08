# TC02 – Invalid Email (Missing Domain) – Automation

## Scenario
Validate that Koel displays the correct error message when the user enters an email address missing the domain.

## Related Manual Test Case
- TC02-invalid-email-missing-domain.md

## Related Bug Report
- BR02-missing-domain-error-not-shown.md

## Automation Logic
- Navigate to https://qa.koel.app/
- Enter invalid email: test@
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
Only the browser’s native HTML5 tooltip appears, which cannot be located via Selenium.

## Evidence
- Screenshot: Browser tooltip displayed
- Screenshot: IntelliJ test execution
- Screenshot: Login page with invalid email entered
