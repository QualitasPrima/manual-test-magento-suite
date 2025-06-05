# Test Case: TC_PDP_CART_003 - Add to Cart - Attempt to Add Out-of-Stock Product

* **Module:** Product Detail Page
* **Feature:** Add to Cart
* **Objective:** Verify system behavior when attempting to add an out-of-stock product to the cart.
* **Priority:** High

**Preconditions:**
1.  User is on the PDP of a product that is explicitly marked as "Out of Stock". (Requires finding/setting up such a product).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the product status and "Add to Cart" button.                                  | Product is "Out of Stock"                     | 1. "Out of Stock" message is clearly displayed. <br> 2. The "Add to Cart" button is disabled. <br> OR <br> 3. If button is somehow enabled, clicking it results in an error message and product not being added. |                                  |                           |                          |
| 2      | If "Add to Cart" button is clickable (unlikely for OOS), click it.                    | -                                             | Product is not added to cart. An appropriate error message about stock availability is displayed.                                               |                                  |                           |                          |
