# Test Case: TC_PDP_CART_001 - Add to Cart - Simple Product with Default Quantity

* **Module:** Product Detail Page
* **Feature:** Add to Cart
* **Objective:** Verify that a simple product (no options) can be successfully added to the cart with the default quantity (usually 1).
* **Priority:** Critical

**Preconditions:**
1.  User is on the PDP of an in-stock simple product (e.g., "Joust Duffle Bag").
2.  Shopping cart is empty or has other items.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Ensure quantity is at the default (e.g., "1").                                        | Quantity: 1                                   | Quantity field shows "1".                                                                                                                     |                                  |                           |                          |
| 2      | Click the "Add to Cart" button.                                                       | -                                             | 1. A success message is displayed (e.g., "You added Joust Duffle Bag to your shopping cart."). <br> 2. The mini-cart icon in the header updates to reflect the added item/quantity. |                                  |                           |                          |
