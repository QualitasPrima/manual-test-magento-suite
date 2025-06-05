# Test Case: TC_CO_SHIPADDR_004 - Shipping Address - Fields with Very Long Strings

* **Module:** Checkout Process
* **Feature:** Shipping Address Input
* **Objective:** Verify system behavior when very long strings are entered into address fields (Street, City).
* **Priority:** Low

**Preconditions:**
1.  User is on the Shipping Address step, adding a new address.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Enter a very long string (e.g., 200+ chars) into "Street Address Line 1".             | Street: `[String of 200+ 'A's]`               | Long string entered.                                                                                                                          |                                  |                           |                          |
| 2      | Enter a very long string into "City". Fill other fields correctly.                    | City: `[String of 100+ 'B's]`                 | Long string entered.                                                                                                                          |                                  |                           |                          |
| 3      | Click "Next".                                                                         | -                                             | 1. System accepts the input (possibly truncating it on backend or display later). <br> OR <br> 2. A validation error appears if there's a character limit per field. <br> System should handle gracefully without crashing. |                                  |                           |                          |
