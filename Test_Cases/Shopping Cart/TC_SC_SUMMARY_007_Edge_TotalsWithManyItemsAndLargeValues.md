# Test Case: TC_SC_SUMMARY_007 - Summary - Totals with Many Items and/or Large Price Values

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify the cart summary calculations and display formatting for a cart with a large number of items or items with very high prices, leading to large subtotals/order totals.
* **Priority:** Low

**Preconditions:**
1.  User has added multiple items to the cart, or a few very high-priced items, such that the Order Total is a large number (e.g., > $10,000.00 or many line items). (May require conceptual items for testing).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Add items to achieve a large subtotal/order total.                                    | e.g., 50 items x $200 each, or 1 item at $15,000 | Cart is populated.                                                                                                                            |                                  |                           |                          |
| 2      | Observe the "Summary" section, focusing on Subtotal and Order Total.                  | -                                             | 1. The Subtotal and Order Total are calculated correctly, even for large numbers. <br> 2. The currency formatting is maintained (e.g., correct decimal places, currency symbol, thousand separators if applicable for the locale). <br> 3. The summary section layout is not broken by the large numbers. |                                  |                           |                          |
| 3      | Perform an action that forces recalculation (e.g., update quantity of one item slightly). | Update qty of one item                        | Totals recalculate correctly and formatting remains intact.                                                                                   |                                  |                           |                          |
