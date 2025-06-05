# Test Case: TC_PDP_QTY_001 - Quantity - Update Quantity via Input Field

* **Module:** Product Detail Page
* **Feature:** Quantity Input
* **Objective:** Verify that the user can successfully update the product quantity by typing a valid number into the quantity input field.
* **Priority:** High

**Preconditions:**
1.  User is on a PDP. Default quantity is usually "1".

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Locate the quantity input field.                                                      | -                                             | Quantity field is visible, displaying "1" by default.                                                                                         |                                  |                           |                          |
| 2      | Click into the quantity field, clear the existing value, and type a new valid quantity. | New Quantity: `3`                             | The number "3" is displayed in the quantity field.                                                                                            |                                  |                           |                          |
| 3      | Click outside the field or proceed to Add to Cart.                                    | -                                             | The quantity remains "3". (Some sites might have +/- buttons that also reflect this change or can be used).                                 |                                  |                           |                          |
