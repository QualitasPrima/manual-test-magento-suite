# Test Case: TC_SC_REMOVE_002 - Remove Item - Remove the Last Item from Cart

* **Module:** Shopping Cart
* **Feature:** Remove Item
* **Objective:** Verify that removing the last remaining item empties the cart and displays the empty cart message.
* **Priority:** High

**Preconditions:**
1.  Cart contains only one item (Product A).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Click the "Remove" icon/link for Product A.                                           | Remove Product A                              | 1. Product A is removed. <br> 2. The cart page updates to show the "empty cart" message (e.g., "You have no items in your shopping cart."). <br> 3. Cart totals are $0.00 or not displayed. |                                  |                           |                          |
