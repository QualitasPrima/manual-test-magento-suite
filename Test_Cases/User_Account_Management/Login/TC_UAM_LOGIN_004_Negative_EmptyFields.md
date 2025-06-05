# Test Case: TC_UAM_LOGIN_004 - Login - Empty Email and Password Fields

* **Module:** User Account Management
* **Feature:** Login
* **Objective:** Verify that login fails and appropriate error messages are displayed when attempting to log in with empty email and password fields.
* **Priority:** Medium

**Preconditions:**
1.  User is on the "Customer Login" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable) | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Leave the "Email" field empty.                                                        | -                         | Email field is empty.                                                                                                                         |                                  |                           |                          |
| 2      | Leave the "Password" field empty.                                                     | -                         | Password field is empty.                                                                                                                      |                                  |                           |                          |
| 3      | Click the "Sign In" button.                                                           | -                         | 1. Login fails. <br> 2. User remains on the login page. <br> 3. Error messages "This is a required field." are displayed below both the Email and Password fields. |                                  |                           |                          |
