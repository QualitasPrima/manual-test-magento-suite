# Test Case: TC_SC_SUMMARY_002 - Summary - Verify Totals After Item Removal

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify that Subtotal and Order Total update correctly after an item is removed from the cart.
* **Priority:** Critical

**Preconditions:**
1.  Cart has two items: Product A (Price $10, Qty 1), Product B (Price $20, Qty 1). Subtotal=$30, Order Total=$30.
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Remove Product A from the cart.                                                       | Remove Product A                              | Product A is removed. Page updates.                                                                                                           |                                  |                           |                          |
| 2      | Observe the "Summary" section.                                                        | -                                             | 1. Subtotal is displayed as $20.00 (reflecting only Product B). <br> 2. Order Total is displayed as $20.00.                                   |                                  |                           |                          |
