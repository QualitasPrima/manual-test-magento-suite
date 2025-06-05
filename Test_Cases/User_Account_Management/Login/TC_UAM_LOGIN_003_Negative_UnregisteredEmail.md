# Test Case: TC_UAM_LOGIN_003 - Login - Unregistered Email Address

* **Module:** User Account Management
* **Feature:** Login
* **Objective:** Verify that login fails and an appropriate error message is displayed when an unregistered email address is used.
* **Priority:** High

**Preconditions:**
1.  The email `unregistered[timestamp]@example.com` is not registered on the site.
2.  User is on the "Customer Login" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Enter an unregistered email address in the "Email" field.                             | `unregistered[timestamp]@example.com`          | Email is entered.                                                                                                                             |                                  |                           |                          |
| 2      | Enter any password in the "Password" field.                                           | `AnyPassword123`                              | Password is entered.                                                                                                                          |                                  |                           |                          |
| 3      | Click the "Sign In" button.                                                           | -                                             | 1. Login fails. <br> 2. Error message like "The account sign-in was incorrect..." is displayed. (Magento often gives a generic message for security). |                                  |                           |                          |
