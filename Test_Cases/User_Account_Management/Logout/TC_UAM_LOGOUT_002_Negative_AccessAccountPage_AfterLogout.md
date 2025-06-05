# Test Case: TC_UAM_LOGOUT_002 - Logout - Attempt to Access Account-Specific Page After Logout

* **Module:** User Account Management
* **Feature:** Logout (Post-Logout State)
* **Objective:** Verify that a logged-out user cannot access account-specific pages (e.g., My Dashboard) and is redirected to the login page.
* **Priority:** High

**Preconditions:**
1.  User was logged in and has just successfully logged out.
2.  The URL for an account-specific page (e.g., Customer Dashboard) is known. (e.g., `.../customer/account/`)

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | After logging out, attempt to navigate directly to an account-specific page URL.        | e.g., `https://magento.softwaretestingboard.com/customer/account/` | User is redirected to the "Customer Login" page. The account-specific page content is not displayed.                                      |                                  |                           |                          |
| 2      | (Optional) Attempt to use the browser's "Back" button to return to an authenticated page seen before logout. | -                                             | User is redirected to the login page or a public page; authenticated content is not displayed.                                                |                                  |                           |                          |
