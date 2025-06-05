# Test Case: TC_SC_QTY_002 - Quantity - Decrease Item Quantity and Verify Totals

* **Module:** Shopping Cart
* **Feature:** Update Quantity
* **Objective:** Verify that decreasing the quantity (not to zero) of an item in the cart updates subtotals correctly.
* **Priority:** High

**Preconditions:**
1.  User has one item in the cart with Qty=3 (e.g., Product A at $10, item subtotal $30).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note current quantity (3), item subtotal ($30), and Order Subtotal ($30).             | Product A: Qty 3, Price $10                   | Values noted.                                                                                                                                 |                                  |                           |                          |
| 2      | Change the quantity for Product A from 3 to 2.                                        | New Qty: 2                                    | Quantity field for Product A shows 2.                                                                                                         |                                  |                           |                          |
| 3      | Click "Update Shopping Cart" (or wait for auto-update).                               | -                                             | 1. Page updates. <br> 2. Item subtotal for Product A updates to $20 (2 x $10). <br> 3. Cart Order Subtotal updates to $20.                  |                                  |                           |                          |
