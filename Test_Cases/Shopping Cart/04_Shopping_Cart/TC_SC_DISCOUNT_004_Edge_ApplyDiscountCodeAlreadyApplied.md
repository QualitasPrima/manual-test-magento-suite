# Test Case: TC_SC_DISCOUNT_004 - Discount - Attempt to Apply Same Valid Discount Code Twice

* **Module:** Shopping Cart
* **Feature:** Apply Discount Code
* **Objective:** Verify system behavior when a user attempts to apply the same valid discount code that has already been successfully applied.
* **Priority:** Medium

**Preconditions:**
1.  A valid discount code (e.g., "SAVE10") has already been successfully applied to the cart.
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Discount "SAVE10" is already applied, Order Total reflects this discount.             | -                                             | Discount shown in summary.                                                                                                                    |                                  |                           |                          |
| 2      | Re-enter the same valid discount code "SAVE10" into the input field.                  | Discount Code: `SAVE10`                       | Code is entered.                                                                                                                              |                                  |                           |                          |
| 3      | Click "Apply Discount".                                                               | -                                             | 1. An error/info message is displayed (e.g., "Coupon code '[SAVE10]' was already applied."). <br> 2. The discount is not applied a second time. <br> 3. Order Total remains unchanged from its already discounted value. |                                  |                           |                          |
