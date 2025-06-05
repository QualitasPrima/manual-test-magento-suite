# Test Case: TC_SC_SUMMARY_001 - Summary - Verify Totals After Item Quantity Update

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify that the Subtotal and Order Total in the cart summary accurately reflect changes after an item's quantity is updated.
* **Priority:** Critical

**Preconditions:**
1.  Cart has one item: Product A (Price $10, Qty 1). Subtotal=$10, Order Total=$10.
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Update quantity of Product A from 1 to 3.                                             | New Qty for Product A: 3                      | Item subtotal for Product A becomes $30.                                                                                                      |                                  |                           |                          |
| 2      | Click "Update Shopping Cart".                                                         | -                                             | Page updates.                                                                                                                                 |                                  |                           |                          |
| 3      | Observe the "Summary" section.                                                        | -                                             | 1. Subtotal is displayed as $30.00. <br> 2. Order Total is displayed as $30.00 (assuming no tax/shipping yet).                                 |                                  |                           |                          |
| 4      | Add a second item: Product B (Price $20, Qty 1). Update cart.                         | Add Product B (Price $20, Qty 1)              | Item subtotal Product A=$30, Product B=$20.                                                                                                    |                                  |                           |                          |
| 5      | Observe the "Summary" section.                                                        | -                                             | 1. Subtotal is displayed as $50.00. <br> 2. Order Total is displayed as $50.00.                                                                 |                                  |                           |                          |
