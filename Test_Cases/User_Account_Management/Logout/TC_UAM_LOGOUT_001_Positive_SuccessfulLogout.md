# Test Case: TC_UAM_LOGOUT_001 - Logout - Successful Logout

* **Module:** User Account Management
* **Feature:** Logout
* **Objective:** Verify that a logged-in user can successfully log out of their account.
* **Priority:** Critical

**Preconditions:**
1.  User is currently logged in to their account.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable) | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Click on the down arrow next to the user's welcome message/name in the header.        | -                         | A dropdown menu appears with options like "My Account", "My Wish List", "Sign Out".                                                           |                                  |                           |                          |
| 2      | Click on the "Sign Out" link from the dropdown menu.                                  | -                         | 1. User is logged out. <br> 2. User is redirected to the Luma Logout Success page (or homepage). <br> 3. "Sign In" and "Create an Account" links are visible in the header. <br> 4. User-specific welcome message is gone. |                                  |                           |                          |
