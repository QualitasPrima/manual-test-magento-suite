# Test Case: TC_UAM_REG_004 - Registration - Attempt with Weak Password

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify that the system prevents account creation if the password does not meet complexity requirements and displays an appropriate error message.
* **Priority:** High

**Preconditions:**
1.  User is not logged in and is on the "Create New Customer Account" page.
2.  The site has password complexity rules (e.g., min length, mix of character types).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Create New Customer Account" page.                                   | -                                             | Page loads successfully.                                                                                                                      |                                  |                           |                          |
| 2      | Enter valid first name, last name, and a unique email.                                | FN: `Weak`, LN: `Pass`, Email: `weakpass[timestamp]@example.com` | Details are entered.                                                                                                                          |                                  |                           |                          |
| 3      | Enter a password that violates complexity rules (e.g., too short, no numbers/symbols).  | `pass`                                        | Weak password entered.                                                                                                                        |                                  |                           |                          |
| 4      | Confirm the weak password.                                                            | `pass`                                        | Weak password confirmed.                                                                                                                      |                                  |                           |                          |
| 5      | Click the "Create an Account" button.                                                 | -                                             | 1. Account creation fails. <br> 2. User remains on the registration page. <br> 3. An error message indicating password requirements is displayed (e.g., "Minimum of different classes of characters..."). |                                  |                           |                          |
