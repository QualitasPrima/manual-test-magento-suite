# Test Case: TC_SC_SUMMARY_003 - Summary - Verify Totals After Successful Discount Application

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify that the Subtotal, Discount amount, and Order Total in the cart summary are accurately displayed and calculated after a valid discount code is applied.
* **Priority:** High

**Preconditions:**
1.  Cart has items totaling a known Subtotal (e.g., Product A, Price $50, Qty 1; Subtotal = $50).
2.  A valid discount code is known (e.g., "SAVE10" for 10% off).
3.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note the current Subtotal ($50) and Order Total ($50).                                | -                                             | Values noted. No discount is currently applied.                                                                                               |                                  |                           |                          |
| 2      | Apply the valid discount code "SAVE10".                                               | Discount Code: `SAVE10`                       | Discount code is accepted. Page updates.                                                                                                      |                                  |                           |                          |
| 3      | Observe the "Summary" section.                                                        | -                                             | 1. Subtotal remains $50.00. <br> 2. A "Discount (SAVE10)" line item appears showing -$5.00 (10% of $50). <br> 3. Order Total is correctly updated to $45.00. |                                  |                           |                          |
