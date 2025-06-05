# Test Case: TC_PDP_QTY_002 - Quantity - Attempt to Enter Zero Quantity

* **Module:** Product Detail Page
* **Feature:** Quantity Input
* **Objective:** Verify system behavior when a user attempts to set the quantity to zero.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PDP.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In the quantity field, attempt to enter "0".                                          | Quantity: `0`                                 | Behavior depends on implementation: <br> 1. Input might be prevented, or field reverts to "1". <br> OR <br> 2. An error message might appear upon trying to Add to Cart / leaving field. <br> (Luma's field usually enforces min 1 via HTML5 attributes or JS, often reverting if invalid). |                                  |                           |                          |
| 2      | If "0" was accepted in field, attempt to Add to Cart.                                 | -                                             | Product is not added. An error message related to invalid quantity appears, or Add to Cart button is disabled.                                |                                  |                           |                          |
