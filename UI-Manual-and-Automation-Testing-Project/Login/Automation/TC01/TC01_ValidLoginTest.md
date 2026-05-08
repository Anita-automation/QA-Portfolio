# TC01 – Valid Email and Password – Automation

## Scenario
Validate that Koel successfully logs in a user with a valid email and correct password.

## Related Manual Test Case
- TC01-valid-email-password.md

## Automation Logic
- Navigate to https://qa.koel.app/
- Enter valid registered email: anita.surewicz@testpro.io
- Enter correct password
- Click “Log In”
- Assert:
  - User is successfully logged in
  - User is redirected to the Homepage

## Automation Result
- Confirmed: User successfully logged in
- Confirmed: User was redirected to the Homepage

## Reason
This test validates the positive login flow and confirms that Koel correctly authenticates valid credentials.

## Evidence
- Screenshot: Login page with valid credentials entered
- Screenshot: IntelliJ test execution (PASSED)
- Screenshot: Koel Homepage after successful login
