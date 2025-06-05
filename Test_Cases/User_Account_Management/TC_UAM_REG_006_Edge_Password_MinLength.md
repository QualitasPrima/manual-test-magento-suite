# Test Case: TC_UAM_REG_006 - Registration - Password at Exact Minimum Length

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify successful account creation with a password that meets the exact minimum length and complexity requirements.
* **Priority:** Medium

**Preconditions:**
1.  User is not logged in and is on the "Create New Customer Account" page.
2.  The site's minimum password length is known (e.g., 8 characters with 3 character classes for Luma).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Create New Customer Account" page.                                   | -                                             | Page loads successfully.                                                                                                                      |                                  |                           |                          |
| 2      | Enter valid first name, last name, and a unique email.                                | FN: `Min`, LN: `PassEdge`, Email: `minpass[timestamp]@example.com` | Details are entered.                                                                                                                          |                                  |                           |                          |
| 3      | Enter a password that meets the exact minimum length and complexity (e.g., 8 chars, 3 classes). | `P@sswd12` (assuming 8 char min)              | Password entered.                                                                                                                             |                                  |                           |                          |
| 4      | Confirm the password.                                                                 | `P@sswd12`                                                    | Password confirmed.                                                                                                                           |                                  |                           |                          |
| 5      | Click the "Create an Account" button.                                                 | -                                                             | 1. Account is created successfully. <br> 2. User is redirected to "My Dashboard". <br> 3. Success message is displayed.                       |                                  |                           |                          |
