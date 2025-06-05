# Test Case: TC_SC_SUMMARY_006 - Summary - Order Total Becomes Zero (or Negative if Possible)

* **Module:** Shopping Cart
* **Feature:** Cart Summary & Totals
* **Objective:** Verify the cart summary display when the Order Total becomes $0.00 (e.g., due to a 100% discount) or, if theoretically possible, negative.
* **Priority:** Medium

**Preconditions:**
1.  Cart has items (e.g., Product A, Price $20).
2.  A discount code or promotion exists that could make the Order Total $0.00 or (less likely) negative. (Assume "FREEITEM" code makes order total $0.00).
3.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Apply the discount code "FREEITEM".                                                   | Discount Code: `FREEITEM`                     | Discount applied. Page updates.                                                                                                               |                                  |                           |                          |
| 2      | Observe the "Summary" section.                                                        | -                                             | 1. Subtotal shows original item value (e.g., $20.00). <br> 2. Discount line shows the full discount amount (e.g., -$20.00). <br> 3. Order Total correctly displays $0.00. <br> 4. If a scenario could lead to a negative total (very rare for e-commerce), ensure it's handled gracefully (e.g., clamps at $0.00 or shows error, rather than a negative value unless intended). |                                  |                           |                          |
