# Test Case: TC_PDP_QTY_003 - Quantity - Attempt to Enter Non-Numeric or Negative Quantity

* **Module:** Product Detail Page
* **Feature:** Quantity Input
* **Objective:** Verify system behavior when non-numeric or negative values are entered into the quantity field.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PDP.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In the quantity field, attempt to enter non-numeric text.                             | Quantity: `abc`                               | Behavior depends on implementation: <br> 1. Input might be prevented entirely for non-numeric chars. <br> OR <br> 2. Field might clear or revert to previous valid value (e.g., "1"). <br> (Luma's HTML5 number input prevents direct typing of letters). |                                  |                           |                          |
| 2      | In the quantity field, attempt to enter a negative number.                            | Quantity: `-5`                                | Behavior depends on implementation: <br> 1. Input might be prevented, or field reverts to "1". <br> OR <br> 2. Value might change to positive equivalent or a min value like 1. |                                  |                           |                          |
| 3      | If invalid value was accepted in field, attempt to Add to Cart.                       | -                                             | Product is not added. An error message related to invalid quantity appears.                                                                   |                                  |                           |                          |
