# Test Case: TC_PDP_CART_005 - Add to Cart - Rapid Multiple Clicks on "Add to Cart" Button

* **Module:** Product Detail Page
* **Feature:** Add to Cart
* **Objective:** Verify system behavior when "Add to Cart" button is clicked multiple times rapidly.
* **Priority:** Medium

**Preconditions:**
1.  User is on PDP of an in-stock product.
2.  Product options (if any) are selected, quantity is 1.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Click the "Add to Cart" button two or three times in very quick succession.           | -                                             | 1. Product is added to the cart ONLY ONCE with the specified quantity (e.g., 1 item). <br> OR <br> 2. Product is added once, subsequent clicks might be disabled temporarily or show a message that item is already added/updated. <br> 3. The system does not add multiple instances of the same intended single addition or crash. Cart quantity should be correct. |                                  |                           |                          |
| 2      | Check the mini-cart quantity for the product.                                         | -                                             | Mini-cart shows the correct quantity (e.g., 1 item, not 2 or 3 from rapid clicks for a single intended item addition).                      |                                  |                           |                          |
