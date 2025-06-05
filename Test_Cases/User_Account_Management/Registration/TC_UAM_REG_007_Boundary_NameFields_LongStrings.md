# Test Case: TC_UAM_REG_007 - Registration - Name Fields with Very Long Strings

* **Module:** User Account Management
* **Feature:** Create Account (Registration)
* **Objective:** Verify system behavior when very long strings are entered into First Name and Last Name fields (check for truncation, errors, or acceptance).
* **Priority:** Low

**Preconditions:**
1.  User is not logged in and is on the "Create New Customer Account" page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Create New Customer Account" page.                                   | -                                             | Page loads successfully.                                                                                                                      |                                  |                           |                          |
| 2      | Enter a very long string (e.g., 256+ characters) in the "First Name" field.           | `[Long string of 260 'A's]`                                   | Long string entered.                                                                                                                          |                                  |                           |                          |
| 3      | Enter a very long string (e.g., 256+ characters) in the "Last Name" field.            | `[Long string of 260 'B's]`                                   | Long string entered.                                                                                                                          |                                  |                           |                          |
| 4      | Enter a unique email, and valid password details.                                     | Email: `longname[timestamp]@example.com`, Pass: `Password123!` | Details are entered.                                                                                                                          |                                  |                           |                          |
| 5      | Click the "Create an Account" button.                                                 | -                                             | Observe behavior: <br> 1. Account creation might succeed (names might be truncated by backend or UI). <br> OR <br> 2. An error message regarding name length might be displayed. <br> (Expected: System handles gracefully, ideally with truncation or clear error if limits exist and are exceeded). |                                  |                           |                          |
