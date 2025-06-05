# Test Case: TC_UAM_REG_005 - Registration - Attempt with Mismatched Passwords

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify that the system prevents account creation if the "Password" and "Confirm Password" fields do not match and displays an appropriate error message.
* **Priority:** High

**Preconditions:**
1.  User is not logged in and is on the "Create New Customer Account" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Create New Customer Account" page.                                   | -                                             | Page loads successfully.                                                                                                                      |                                  |                           |                          |
| 2      | Enter valid first name, last name, and a unique email.                                | FN: `Mismatch`, LN: `User`, Email: `mismatch[timestamp]@example.com` | Details are entered.                                                                                                                          |                                  |                           |                          |
| 3      | Enter a strong password in the "Password" field.                                      | `PasswordGood1!`                                              | Password entered.                                                                                                                             |                                  |                           |                          |
| 4      | Enter a different password in the "Confirm Password" field.                           | `PasswordBad2@`                                               | Different password confirmed.                                                                                                                 |                                  |                           |                          |
| 5      | Click the "Create an Account" button.                                                 | -                                             | 1. Account creation fails. <br> 2. User remains on the registration page. <br> 3. An error message like "Please enter the same value again." is displayed for the Confirm Password field. |                                  |                           |                          |
