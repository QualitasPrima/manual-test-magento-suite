# Test Case: TC_CO_SHIPADDR_003 - Shipping Address - Invalid Zip/Postal Code Format

* **Module:** Checkout Process
* **Feature:** Shipping Address Validation
* **Objective:** Verify error handling for invalid Zip/Postal Code formats based on the selected country/state.
* **Priority:** Medium

**Preconditions:**
1.  User is on the Shipping Address step. Country "United States" and a State are selected.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Fill all other mandatory fields. Enter an obviously incorrect Zip Code format for US. | Zip Code: `ABCDE` or `123` (for US)         | Invalid Zip Code entered.                                                                                                                     |                                  |                           |                          |
| 2      | Click "Next".                                                                         | -                                             | 1. User is not navigated. <br> 2. An error message related to invalid Zip Code format for the selected region is displayed. (e.g., "Provided Zip/Postal Code is incorrect..."). Or, the field might have specific format enforcement client-side. |                                  |                           |                          |
