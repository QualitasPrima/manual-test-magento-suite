# Test Case: TC_SC_DISCOUNT_003 - Discount - Attempt to Apply Empty Discount Code

* **Module:** Shopping Cart
* **Feature:** Apply Discount Code
* **Objective:** Verify system behavior (ideally an error message or no action) when attempting to apply an empty discount code.
* **Priority:** Medium

**Preconditions:**
1.  User has item(s) in the cart. User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Leave the discount code input field empty.                                            | Discount Code: (empty)                        | Field is empty.                                                                                                                               |                                  |                           |                          |
| 2      | Click "Apply Discount".                                                               | -                                             | 1. An error message might appear (e.g., "Please enter a coupon code."). <br> OR <br> 2. The button click might do nothing if client-side validation prevents submission of empty field. <br> 3. No discount applied, totals unchanged. |                                  |                           |                          |
