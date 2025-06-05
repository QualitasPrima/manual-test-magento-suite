# Test Case: TC_CO_SHIPADDR_002 - Shipping Address - Invalid Email Format (Guest Checkout)

* **Module:** Checkout Process
* **Feature:** Shipping Address Validation (Guest)
* **Objective:** Verify that an invalid email format entered by a guest user on the shipping address step triggers an error message.
* **Priority:** High

**Preconditions:**
1.  User is a guest and on the Shipping Address step.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Fill all other mandatory shipping fields. Enter an invalid email format in the Email field. | Email: `invalid-email`, `test@.com`, `test@domain` | Invalid email format entered.                                                                                                                 |                                  |                           |                          |
| 2      | Click "Next".                                                                         | -                                             | 1. User is not navigated. <br> 2. An error message like "Please enter a valid email address (Ex: johndoe@domain.com)." is displayed for the Email field. |                                  |                           |                          |
