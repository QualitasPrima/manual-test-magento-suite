# Test Case: TC_SC_SUMMARY_004 - Summary - Verify Totals Remain Unchanged After Failed Discount Application

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify that if an attempt to apply an invalid discount code fails, the cart summary (Subtotal, Discount, Order Total) remains unchanged from its pre-attempt state.
* **Priority:** Medium

**Preconditions:**
1.  Cart has items with a known Subtotal and Order Total (e.g., $50).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note the current Subtotal ($50) and Order Total ($50).                                | -                                             | Values noted. No discount is applied.                                                                                                         |                                  |                           |                          |
| 2      | Attempt to apply an invalid discount code.                                            | Discount Code: `INVALIDCODE`                  | An error message "The coupon code '[INVALIDCODE]' is not valid." is displayed.                                                                  |                                  |                           |                          |
| 3      | Observe the "Summary" section after the failed attempt.                               | -                                             | 1. Subtotal remains $50.00. <br> 2. No "Discount" line item is displayed (or any previous valid discount remains, but no new invalid one is applied). <br> 3. Order Total remains $50.00 (or its value before the failed attempt). |                                  |                           |                          |
