# TC03 – Invalid Email (Missing @ Symbol) – Automation

**Scenario**  
Validate that Koel displays the correct error message when the user enters an email address without the @ symbol.

**Related Manual Test Case**  
- TC03-invalid-email-no-at-symbol.md

**Automation Logic**  
- Navigate to https://qa.koel.app/  
- Enter invalid email: anita.surewicztestpro.io  
- Enter valid password  
- Click “Log In”  
- Assert:  
  - User remains on the Login page  
  - (Attempted) Expected Koel validation message: "Email format is incorrect"

**Automation Result**  
- Confirmed: User remained on the Login page  
- Not Confirmed: Expected Koel validation message

**Reason**  
The Koel UI does not render a CSS-selectable element for the validation message.  
Only the browser’s native HTML5 tooltip appears, which cannot be located via Selenium.

**Evidence**  
- Screenshot: Browser tooltip displayed  
- Screenshot: IntelliJ test execution
