# 🐞 UI/UX Bug Report – ORANGEHRM_UI_BUG_001

## Title
Profile dropdown does not toggle closed when clicking the profile icon again

---

## Application
OrangeHRM – Open Source Demo

## Version
5.8

## Module
User Profile / Header Navigation

## Environment
- Platform: Windows
- Browser: Google Chrome (latest)
- Testing Type: Manual Testing (UI/UX Validation)

---

## Steps to Reproduce
1. Open the OrangeHRM open-source demo application
2. Login using valid credentials (Admin / admin123)
3. Click on the user profile icon in the top-right corner
4. Observe that the dropdown menu opens
5. Click on the same user profile icon again

---

## Expected Result
Clicking the user profile icon again should close (toggle) the dropdown menu.

---

## Actual Result
The dropdown menu does not close when clicking the profile icon again.  
It only closes when the user clicks outside the dropdown, resulting in inconsistent toggle behavior.

---

## Severity
Minor

## Priority
Medium

---

## Status
Open

---

## Attachments
Screenshot attached highlighting the profile dropdown behavior.

---

## Remarks
This issue affects user experience and expected UI interaction consistency.

---

### Reference
GitHub Issue: https://github.com/orangehrm/orangehrm/issues/1923



