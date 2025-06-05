# Test Case: TC_SC_QTY_005 - Quantity - Attempt to Update Quantity to Exceed Available Stock

* **Module:** Shopping Cart
* **Feature:** Update Quantity
* **Objective:** Verify system behavior when updating an item's quantity in the cart to a value greater than available stock.
* **Priority:** High

**Preconditions:**
1.  User has an item in the cart (e.g., Product X, Qty 1).
2.  Available stock for Product X is known and limited (e.g., 5 units). (Requires finding/setting up such a product).
3.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Change the quantity for Product X to a value greater than available stock (e.g., 10, when stock is 5). | New Qty: 10 (Stock: 5)                      | Quantity field shows 10.                                                                                                                      |                                  |                           |                          |
| 2      | Click "Update Shopping Cart".                                                         | -                                             | 1. An error message is displayed (e.g., "The requested quantity for '[Product X]' is not available."). <br> 2. The quantity for Product X in the cart either reverts to the previous valid quantity (1) or is updated to the maximum available stock (5). <br> 3. Cart totals reflect the actual quantity allowed. |                                  |                           |                          |
