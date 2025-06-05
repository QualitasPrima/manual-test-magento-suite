# Test Case: TC_SC_DISCOUNT_002 - Discount - Apply Invalid or Expired Discount Code

* **Module:** Shopping Cart
* **Feature:** Apply Discount Code
* **Objective:** Verify that an appropriate error message is displayed when an invalid or expired discount code is applied, and totals are not affected.
* **Priority:** High

**Preconditions:**
1.  User has item(s) in the cart. User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Note current Order Total.                                                             | -                                             | Total noted.                                                                                                                                  |                                  |                           |                          |
| 2      | Enter an invalid or expired discount code.                                            | Discount Code: `INVALIDCODE123`               | Code is entered.                                                                                                                              |                                  |                           |                          |
| 3      | Click "Apply Discount".                                                               | -                                             | 1. An error message is displayed (e.g., "The coupon code '[INVALIDCODE123]' is not valid."). <br> 2. No discount is applied. <br> 3. Order Total remains unchanged. |                                  |                           |                          |
