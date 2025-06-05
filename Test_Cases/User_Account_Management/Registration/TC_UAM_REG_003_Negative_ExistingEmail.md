# Test Case: TC_UAM_REG_003 - Registration - Attempt with Existing Email

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify that the system prevents account creation if the provided email address is already registered and displays an appropriate error message.
* **Priority:** Critical

**Preconditions:**
1.  An email address `existinguser@example.com` is already registered on the site. (Assume this for the test; you might need to create one first if testing for real).
2.  User is not logged in and is on the "Create New Customer Account" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Create New Customer Account" page.                                   | -                                             | Page loads successfully.                                                                                                                      |                                  |                           |                          |
| 2      | Enter valid first name and last name.                                                 | FN: `Another`, LN: `User`                     | Names are entered.                                                                                                                            |                                  |                           |                          |
| 3      | Enter the pre-existing email address in the "Email" field.                            | `existinguser@example.com`                    | Email address is entered.                                                                                                                     |                                  |                           |                          |
| 4      | Enter a strong password and confirm it.                                               | `Password123!`                                | Passwords are entered.                                                                                                                        |                                  |                           |                          |
| 5      | Click the "Create an Account" button.                                                 | -                                             | 1. Account creation fails. <br> 2. User remains on the "Create New Customer Account" page. <br> 3. An error message like "There is already an account with this email address..." is displayed. |                                  |                           |                          |
