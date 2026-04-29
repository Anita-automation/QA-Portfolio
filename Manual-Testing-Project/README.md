# Koel App — Artists Feature (Manual UI Testing)

This repository contains manual UI test cases, exploratory testing notes, and bug reports for validating the Artists feature of the Koel music streaming application.

All testing was performed against the Koel QA environment:  
https://qa.koel.app

This work was managed in Jira (Zephyr) as part of a structured QA workflow.

## Project Overview
The goal of this project was to verify that users can browse, search, and play music from multiple artists in the Koel web application.

This work is based on the user story:

“As a user, I want to have multiple artists in the app, so that I can enjoy different music.”

The acceptance criteria required testing:

- Artists are visible in the UI  
- Users can search for artists  
- Users can play a song from a selected artist  
- Artist data matches the database  
- All test cases prepared for future automation  

## What This Repository Contains

### Test Cases
Located in the **Test-Cases** folder.

Each test case includes:

- Objective  
- Preconditions  
- Test Data  
- Steps  
- Expected Result  
- Actual Result  
- Evidence  

The test suite covers:

- Searching for existing artists  
- Playing songs from selected artists  
- Verifying artist information  
- Matching UI data with database records  
- Audio streaming validation  
- Invalid/empty search behaviour  
- Case‑insensitive search  

### Bug Reports
Located in the **Bug-Reports** folder.

Each bug report includes:

- Summary  
- Environment  
- Preconditions  
- Steps to Reproduce  
- Expected vs Actual Result  
- Evidence  

Documented defects include:

- Incorrect search results  
- Artists grouped under “Unknown Artist”  
- UI not matching database records  
- Invalid search returning incorrect results  

## Evidence
All screenshots used in test cases and bug reports are stored in the **Evidence** folder.

## Repository Structure
Koel-Artists-Manual-Testing/
├── Test-Cases/
├── Bug-Reports/
└── Evidence/

## Purpose of This Project
This project demonstrates:

- Manual UI and functional testing  
- Test case design using Jira/Zephyr  
- Exploratory testing  
- Defect reporting with clear reproduction steps  
- Evidence‑based documentation  
- Validation of UI behaviour against database records  
- Organised QA documentation suitable for a professional portfolio 
