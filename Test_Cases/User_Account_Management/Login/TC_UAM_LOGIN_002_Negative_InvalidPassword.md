# Test Case: TC_UAM_LOGIN_002 - Login - Valid Email, Invalid Password

* **Module:** User Account Management
* **Feature:** Login
* **Objective:** Verify that login fails and an appropriate error message is displayed when a registered email is used with an incorrect password.
* **Priority:** High

**Preconditions:**
1.  User has a valid, registered account (e.g., email: `testuserone[timestamp]@example.com`).
2.  User is on the "Customer Login" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Enter the registered email address in the "Email" field.                              | `testuserone[timestamp]@example.com` (use actual created email) | Email is entered.                                                                                                                             |                                  |                           |                          |
| 2      | Enter an incorrect password in the "Password" field.                                  | `WrongPassword123`                                            | Incorrect password is entered.                                                                                                                |                                  |                           |                          |
| 3      | Click the "Sign In" button.                                                           | -                                                             | 1. Login fails. <br> 2. User remains on the login page or is shown a login error message area. <br> 3. An error message like "The account sign-in was incorrect or your account is disabled temporarily. Please wait and try again later." is displayed. |                                  |                           |                          |
