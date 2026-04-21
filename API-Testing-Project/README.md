# Koel API Testing — Get Song Information

This repository contains API test cases, bug reports, and evidence screenshots for validating the Koel music streaming application's **GET /api/song/{song_id}/info** endpoint and related authentication flows.

All testing was performed against the Koel QA environment:  
https://qa.koel.app

This work was managed in **Jira (Zephyr)** as part of a structured QA workflow, and all API calls were executed and validated using **Postman**.

---

## Project Overview

The goal of this project was to verify that a registered user can successfully retrieve song information and that the API correctly enforces authentication and input validation.

This work is based on the user story:

**“As a registered user, I should be able to get song’s info.”**

The acceptance criteria required testing:

- Valid request → **200 OK**
- Missing or invalid token → **401 Unauthorized**
- Missing or incorrect song ID → **404 Not Found**
- Endpoint availability and correct method handling

---

## What This Repository Contains

### Test Cases  
Located in the `Test-Cases` folder.

Each test case includes:

- Objective  
- Preconditions  
- Test Data  
- Steps  
- Expected Result  
- Actual Result  
- Evidence screenshot  

The test suite covers:

- Valid token (positive test)
- Incorrect HTTP method
- Missing song ID
- Wrong/invalid song ID
- Missing Bearer token
- Expired token
- Overly long token
- Incorrect/invalid token

All tests were executed using **Postman**, with authentication handled via Bearer tokens.

---

### Bug Reports  
Located in the `Bug-Reports` folder.

Each bug report includes:

- Summary  
- Environment  
- Preconditions  
- Steps to Reproduce  
- Expected vs Actual Result  
- Screenshot evidence  

These reports document issues such as:

- Invalid or missing tokens returning **200 OK** instead of **401**
- Overly long tokens returning **404 Not Found**
- Authentication not being enforced correctly

All defects were logged and tracked in **Jira (Zephyr)** as part of the project workflow.

---

### Evidence  
All screenshots used in test cases and bug reports are stored in the `Evidence` folder.

---

## Repository Structure

```
API-Testing-Project/
│
├── Test-Cases/
├── Bug-Reports/
└── Evidence/Screenshots/
```

---

## Purpose of This Project

This project demonstrates:

- API testing using Postman  
- Authentication and security validation  
- Negative testing  
- Bug reporting with clear reproduction steps  
- Working within a Jira-managed workflow  
- Organised documentation suitable for a QA portfolio  

It reflects real‑world API testing practices and shows the ability to identify and document defects in authentication logic.
