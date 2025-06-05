# Test Case: TC_UAM_REG_001 - Registration - Successful with Required Fields

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify that a new user can successfully create an account by providing all valid required information.
* **Priority:** Critical

**Preconditions:**
1.  User is not logged in.
2.  User has a unique, valid email address not already registered on the site.
3.  User has chosen a password that meets the site's complexity requirements (e.g., minimum length, character types).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the Luma homepage.                                                        | URL: `https://magento.softwaretestingboard.com/`              | Luma homepage loads successfully.                                                                                                             |                                  |                           |                          |
| 2      | Click on the "Create an Account" link in the header.                                  | -                                                             | User is redirected to the "Create New Customer Account" page.                                                                                 |                                  |                           |                          |
| 3      | Enter a valid first name in the "First Name" field.                                   | `Test`                                                        | First name is entered.                                                                                                                        |                                  |                           |                          |
| 4      | Enter a valid last name in the "Last Name" field.                                     | `UserOne`                                                     | Last name is entered.                                                                                                                         |                                  |                           |                          |
| 5      | Enter a unique, valid email address in the "Email" field.                             | `testuserone[timestamp]@example.com` (replace [timestamp]) | Email address is entered.                                                                                                                     |                                  |                           |                          |
| 6      | Enter a strong password meeting complexity rules in the "Password" field.             | `Password123!`                                                | Password is entered and masked.                                                                                                               |                                  |                           |                          |
| 7      | Re-enter the same password in the "Confirm Password" field.                           | `Password123!`                                                | Password is entered and masked.                                                                                                               |                                  |                           |                          |
| 8      | Click the "Create an Account" button.                                                 | -                                                             | 1. User is redirected to the "My Dashboard" page. <br> 2. A success message "Thank you for registering with Main Website Store." is displayed. <br> 3. User is effectively logged in. |                                  |                           |                          |
