# Test Case: TC_SC_QTY_003 - Quantity - Update Item Quantity to Zero

* **Module:** Shopping Cart
* **Feature:** Update Quantity
* **Objective:** Verify system behavior when an item's quantity in the cart is updated to 0 (item should be removed).
* **Priority:** Medium

**Preconditions:**
1.  User has one item in the cart with Qty=1 (e.g., Product A).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Change the quantity for Product A from 1 to 0.                                        | New Qty: 0                                    | Quantity field for Product A shows 0.                                                                                                         |                                  |                           |                          |
| 2      | Click "Update Shopping Cart" (or wait for auto-update).                               | -                                             | 1. Page updates. <br> 2. Product A is removed from the shopping cart. <br> 3. The cart is now empty (or shows other items if present), and an "empty cart" message may appear. <br> 4. Cart totals update to $0.00 if it was the only item. (Luma removes the item for Qty 0). |                                  |                           |                          |
