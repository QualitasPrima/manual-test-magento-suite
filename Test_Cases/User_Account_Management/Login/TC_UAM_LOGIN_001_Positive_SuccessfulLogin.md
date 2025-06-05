# Test Case: TC_UAM_LOGIN_001 - Login - Successful with Valid Credentials

* **Module:** User Account Management
* **Feature:** Login
* **Objective:** Verify that a registered user can successfully log in with their valid email and password.
* **Priority:** Critical

**Preconditions:**
1.  User has a valid, registered account (e.g., email: `testuserone[timestamp]@example.com`, pass: `Password123!`).
2.  User is logged out and is on the Luma homepage or "Customer Login" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the Luma homepage and click "Sign In", or navigate directly to the login page. | -                                                             | "Customer Login" page is displayed.                                                                                                           |                                  |                           |                          |
| 2      | Enter the registered email address in the "Email" field.                              | `testuserone[timestamp]@example.com` (use actual created email) | Email is entered.                                                                                                                             |                                  |                           |                          |
| 3      | Enter the corresponding valid password in the "Password" field.                       | `Password123!`                                                | Password is entered and masked.                                                                                                               |                                  |                           |                          |
| 4      | Click the "Sign In" button.                                                           | -                                                             | 1. User is successfully logged in. <br> 2. User is redirected to "My Dashboard" or the previous page. <br> 3. Welcome message with user's name is displayed. <br> 4. "Sign Out" link is visible. |                                  |                           |                          |
