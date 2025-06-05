# Test Case: TC_SC_QTY_001 - Quantity - Increase Item Quantity and Verify Totals

* **Module:** Shopping Cart
* **Feature:** Update Quantity
* **Objective:** Verify that increasing the quantity of an item in the cart updates the item's subtotal and the cart's order subtotal/total correctly.
* **Priority:** Critical

**Preconditions:**
1.  User has at least one item in the cart with Qty=1 (e.g., Product A at $10).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note the current quantity (1), item subtotal ($10), and Order Subtotal ($10).         | Product A: Qty 1, Price $10                   | Values noted.                                                                                                                                 |                                  |                           |                          |
| 2      | Locate the quantity input field for Product A. Change the quantity from 1 to 3.       | New Qty: 3                                    | Quantity field for Product A shows 3.                                                                                                         |                                  |                           |                          |
| 3      | Click the "Update Shopping Cart" button (or wait for auto-update if applicable).      | -                                             | 1. Page reloads/updates. <br> 2. Item subtotal for Product A updates to $30 (3 x $10). <br> 3. Cart Order Subtotal updates to $30. <br> 4. A success message for cart update may appear. |                                  |                           |                          |
