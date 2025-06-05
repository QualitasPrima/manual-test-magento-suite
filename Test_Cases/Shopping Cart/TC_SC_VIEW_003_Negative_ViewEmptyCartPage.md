# Test Case: TC_SC_VIEW_003 - View Cart - Display of Empty Cart Page

* **Module:** Shopping Cart
* **Feature:** View Cart Contents
* **Objective:** Verify that an appropriate message and layout are displayed when the shopping cart is empty.
* **Priority:** Medium

**Preconditions:**
1.  The shopping cart is empty (either user has not added items, or all items have been removed).
2.  User navigates to the Shopping Cart page (`checkout/cart/`).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the content of the Shopping Cart page.                                        | -                                             | 1. A message indicating the cart is empty is displayed (e.g., "You have no items in your shopping cart."). <br> 2. No product items are listed. <br> 3. The cart summary (Subtotal, Order Total) shows $0.00 or is not displayed. <br> 4. A "Continue Shopping" link/button is prominent. <br> 5. "Proceed to Checkout" button is typically hidden or disabled. |                                  |                           |                          |
