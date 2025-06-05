# Test Case: TC_CO_SHIPADDR_001 - Shipping Address - Proceed with Missing Required Fields

* **Module:** Checkout Process
* **Feature:** Shipping Address Validation
* **Objective:** Verify that the system prevents proceeding from the shipping address step if mandatory fields are left empty and displays appropriate error messages.
* **Priority:** Critical

**Preconditions:**
1.  User (guest or registered adding new address) is on the Shipping Address step of checkout.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Fill in some fields but leave a mandatory field empty (e.g., First Name, Street Address, City, Zip Code, or Phone Number). | e.g., Leave "First Name" blank                | Other fields filled, First Name is empty.                                                                                                     |                                  |                           |                          |
| 2      | Attempt to select a shipping method and click "Next" (or just "Next" if shipping method is on same step for guest before full address). | -                                             | 1. User is NOT navigated to the next step. <br> 2. An error message "This is a required field." (or similar) is displayed next to or below each empty mandatory field. |                                  |                           |                          |
| 3      | Repeat by leaving a different mandatory field empty (e.g., "Street Address"). Click "Next". | Leave "Street Address" blank                  | Error message appears for "Street Address".                                                                                                   |                                  |                           |                          |
