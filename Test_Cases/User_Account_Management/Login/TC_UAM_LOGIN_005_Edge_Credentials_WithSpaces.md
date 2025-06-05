# Test Case: TC_UAM_LOGIN_005 - Login - Credentials with Leading/Trailing Spaces

* **Module:** User Account Management
* **Feature:** Login
* **Objective:** Verify system behavior (successful login if trimmed, or failure if not) when credentials (email/password) are entered with leading/trailing spaces.
* **Priority:** Low

**Preconditions:**
1.  User has a valid, registered account (e.g., email: `trimtest[timestamp]@example.com`, pass: `TrimPass1!`). Assume no leading/trailing spaces in the actual stored credentials.
2.  User is on the "Customer Login" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Enter the registered email with leading and trailing spaces.                          | `  trimtest[timestamp]@example.com  ` (use actual created email) | Email with spaces entered.                                                                                                                    |                                  |                           |                          |
| 2      | Enter the correct password with leading and trailing spaces.                          | `  TrimPass1!  `                                               | Password with spaces entered.                                                                                                                 |                                  |                           |                          |
| 3      | Click the "Sign In" button.                                                           | -                                                             | Observe behavior: <br> 1. **Ideal:** Login is successful (system trims spaces). <br> OR <br> 2. Login fails (system does not trim spaces and treats them as part of credentials). <br> (Expected: Successful login due to trimming is common, but failure is also possible depending on implementation). |                                  |                           |                          |
