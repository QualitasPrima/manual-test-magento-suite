# Test Case: TC_SC_QTY_004 - Quantity - Attempt to Update Quantity to Non-Numeric Value

* **Module:** Shopping Cart
* **Feature:** Update Quantity
* **Objective:** Verify system behavior when a non-numeric value is entered into an item's quantity field in the cart.
* **Priority:** Medium

**Preconditions:**
1.  User has an item in the cart. User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Attempt to type a non-numeric value (e.g., "abc") into the quantity field for an item. | New Qty: "abc"                                | 1. Input of non-numeric characters is prevented by the field (HTML5 number type). <br> OR <br> 2. If input is allowed, upon clicking "Update Shopping Cart", an error message appears, and quantity is not updated/reverts to previous valid value. |                                  |                           |                          |
| 2      | Attempt to type a negative value (e.g., "-2") into the quantity field.                | New Qty: "-2"                                 | 1. Input of negative sign may be prevented. <br> OR <br> 2. If input allowed, on update, error message appears or value reverts/is corrected (e.g. to 1 or previous value). |                                  |                           |                          |
