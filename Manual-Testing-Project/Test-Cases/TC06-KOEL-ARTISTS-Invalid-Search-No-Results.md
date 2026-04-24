# Test Case: Koel | Artists | Search returns no results for invalid artist

## Objective
Verify that the Artists search functionality correctly displays **no results** when the user enters an invalid or non‑existent artist name.

## Preconditions
- Valid Koel user account  
- User is logged into Koel: https://qa.koel.app/#!/home  
- User is on the Artists page or Home page with the search bar visible  

## Test Data
- Invalid artist name: **"Bongo bongo"**

## Steps
1. Log into Koel  
2. Click on the search field  
3. Enter an invalid artist name: **"Bongo bongo"**  
4. Observe the displayed results under:
   - Songs  
   - Artists  
   - Albums  

## Expected Result
- No matching artists should be displayed  
- No matching songs should be displayed  
- No matching albums should be displayed  
- A clear **“None found”** or equivalent empty‑state message should appear in each section  

## Actual Result
- **Songs:** Displays *“None found”* correctly  
- **Artists:** Incorrectly displays an unrelated artist (**Metre**)  
- **Albums:** Incorrectly displays an unrelated album (**Chevalerie EP by AKMV‑18**)  
- Search results do **not** reflect the invalid query  
- System returns **false positives** instead of an empty result set  

## Status
❌ **Failed**

## Evidence
- Screenshot: TC02‑1 (invalid search returns unrelated results)  
- Related Bug Report: *To be created* (e.g., **BR02‑ARTISTS‑Invalid‑Search‑Returns‑Incorrect‑Results.md**)
