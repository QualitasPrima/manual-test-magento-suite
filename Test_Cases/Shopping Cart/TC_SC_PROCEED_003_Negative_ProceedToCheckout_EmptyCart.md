# Test Case: TC_SC_PROCEED_003 - Proceed - Attempt to Proceed to Checkout with an Empty Cart

* **Module:** Shopping Cart
* **Feature:** Proceed to Checkout
* **Objective:** Verify the behavior of the "Proceed to Checkout" functionality when the shopping cart is empty.
* **Priority:** Medium

**Preconditions:**
1.  The shopping cart is empty.
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the "Proceed to Checkout" button.                                             | -                                             | The "Proceed to Checkout" button is either: <br> 1. Disabled. <br> OR <br> 2. Hidden entirely. <br> OR <br> 3. If clickable, it does not proceed and may show a message "Cart is empty". |                                  |                           |                          |
| 2      | If the button is clickable, click it.                                                 | -                                             | User is not navigated to the checkout process. An appropriate message about the empty cart might be displayed, or no action occurs if disabled. |                                  |                           |                          |
