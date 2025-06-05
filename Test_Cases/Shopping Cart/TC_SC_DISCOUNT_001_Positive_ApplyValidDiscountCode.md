# Test Case: TC_SC_DISCOUNT_001 - Discount - Apply Valid Discount Code

* **Module:** Shopping Cart
* **Feature:** Apply Discount Code
* **Objective:** Verify that a valid discount code can be applied, and the cart totals are updated correctly to reflect the discount.
* **Priority:** High

**Preconditions:**
1.  User has item(s) in the cart eligible for a known, valid discount code.
2.  User is on the Shopping Cart page.
3.  A valid, active discount code for the Luma demo site is known (e.g., assume "SAVE10" gives 10% off). *Finding actual working demo codes can be tricky; this may be a conceptual test or require setup.*

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note the current Order Subtotal and Order Total.                                      | -                                             | Totals noted.                                                                                                                                 |                                  |                           |                          |
| 2      | Locate the "Apply Discount Code" section/input field.                                 | -                                             | Input field and "Apply Discount" button are visible.                                                                                          |                                  |                           |                          |
| 3      | Enter the valid discount code into the field.                                         | Discount Code: `SAVE10` (example)             | Code is entered.                                                                                                                              |                                  |                           |                          |
| 4      | Click the "Apply Discount" button.                                                    | -                                             | 1. Page updates. <br> 2. A success message may appear indicating the discount was applied. <br> 3. The "Discount" amount is shown in the cart summary. <br> 4. The Order Total is reduced by the discount amount. |                                  |                           |                          |
| 5      | Verify the option to "Cancel" or remove the applied coupon is present.                | -                                             | A link/button like "Cancel Coupon" is visible.                                                                                                |                                  |                           |                          |
