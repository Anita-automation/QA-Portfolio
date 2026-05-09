# Koel App — Login Feature (Manual & Automation Testing)

This repository contains **manual UI test cases**, **Selenium automation tests**, and **bug reports** for validating the **Login functionality** of the Koel music streaming application.

All testing was performed against the Koel QA environment:  
https://qa.koel.app

---

## 📌 Project Overview

The goal of this project was to verify that users can authenticate correctly and that invalid inputs are handled consistently.

**User Story:**  
“As a user, I want to log into the app securely, so that I can access my music.”

**Acceptance criteria included:**

- Successful login with valid credentials  
- Validation of incorrect email formats  
- Validation of incorrect passwords  
- Required‑field behavior  
- Redirecting users back to previously saved pages  
- Preparing all manual tests for future automation  

---

## 📁 Repository Structure

```text
UI-Manual-and-Automation-Testing-Project/
└── Login/
    ├── Manual-Tests/
    │   ├── TC01/
    │   ├── TC02/
    │   ├── TC03/
    │   ├── TC04/
    │   ├── TC05/
    │   ├── TC06/
    │   └── TC07/
    │
    ├── Automation/
    │   ├── TC01/
    │   ├── TC02/
    │   ├── TC03/
    │   ├── TC04/
    │   ├── TC05/
    │   ├── TC06/
    │   └── TC07/
    │
    └── Bug-Reports/
        ├── BR02/
        ├── BR03/
        ├── BR04/
        ├── BR05/
        └── BR06/


## 🧪 Manual Test Cases

Located in **Manual-Tests**.

Each test case includes:

- Objective  
- Preconditions  
- Test Data  
- Steps  
- Expected Result  
- Actual Result  
- Evidence (IntelliJ screenshot only)  
- Traceability (linked at the bottom)

Covers:

- Valid login  
- Invalid email formats  
- Empty fields  
- Incorrect password  
- Login redirect behavior  

---

## 🤖 Automation Tests

Located in **Automation**.

Each automation test includes:

- Scenario  
- Automation Logic  
- Automation Result  
- Reason  
- **Traceability (linked at the top)**  
  - Manual Test  
  - Bug Report (if failed)

Built using:

- Selenium WebDriver  
- Java  
- TestNG  
- Page Object Model (POM)

Automation mirrors the manual suite for full traceability.

---

## 🐞 Bug Reports

Located in **Bug-Reports**.

Each bug report includes:

- Summary  
- Environment  
- Preconditions  
- Steps to Reproduce  
- Expected vs Actual Result  
- Evidence (UI + tooltip + IntelliJ screenshots)  
- Traceability (linked at the bottom)

Documented defects include:

- Missing validation messages for invalid email formats  
- Missing validation for empty fields  
- Missing incorrect‑password error message  

---

## 🎯 Purpose of This Project

This project demonstrates:

- Manual UI and functional testing  
- Test case design aligned with Jira/Zephyr  
- Selenium automation with Java + TestNG  
- Page Object Model (POM) structure  
- Evidence‑based defect reporting  
- Full traceability between manual tests, automation tests, and bug reports  
- Clean, organised QA documentation suitable for a professional portfolio






## 🧪 Manual Test Cases

Located in **Manual-Tests**.

Each test case includes:

- Objective  
- Preconditions  
- Test Data  
- Steps  
- Expected Result  
- Actual Result  
- Evidence (IntelliJ screenshot only)  
- Traceability (linked at the bottom)

Covers:

- Valid login  
- Invalid email formats  
- Empty fields  
- Incorrect password  
- Login redirect behavior  

---

## 🤖 Automation Tests

Located in **Automation**.

Each automation test includes:

- Scenario  
- Automation Logic  
- Automation Result  
- Reason  
- **Traceability (linked at the top)**  
  - Manual Test  
  - Bug Report (if failed)

Built using:

- Selenium WebDriver  
- Java  
- TestNG  
- Page Object Model (POM)

Automation mirrors the manual suite for full traceability.

---

## 🐞 Bug Reports

Located in **Bug-Reports**.

Each bug report includes:

- Summary  
- Environment  
- Preconditions  
- Steps to Reproduce  
- Expected vs Actual Result  
- Evidence (UI + tooltip + IntelliJ screenshots)  
- Traceability (linked at the bottom)

Documented defects include:

- Missing validation messages for invalid email formats  
- Missing validation for empty fields  
- Missing incorrect‑password error message  

---

## 🎯 Purpose of This Project

This project demonstrates:

- Manual UI and functional testing  
- Test case design aligned with Jira/Zephyr  
- Selenium automation with Java + TestNG  
- Page Object Model (POM) structure  
- Evidence‑based defect reporting  
- Full traceability between manual tests, automation tests, and bug reports  
- Clean, organised QA documentation suitable for a professional portfolio
