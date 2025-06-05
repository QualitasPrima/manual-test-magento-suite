# Test Case: TC_SC_REMOVE_001 - Remove Item - Remove One Item from Cart with Multiple Items

* **Module:** Shopping Cart
* **Feature:** Remove Item
* **Objective:** Verify that a specific item can be successfully removed from a cart containing multiple items, and cart totals update.
* **Priority:** Critical

**Preconditions:**
1.  Cart contains at least two different items (Product A, Product B).
2.  User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Identify Product A to be removed. Click the "Remove" icon/link for Product A.         | Remove Product A                              | 1. Confirmation prompt may appear (Luma typically removes directly with an undo option). <br> 2. Product A is removed from the cart list. <br> 3. Product B remains in the cart. <br> 4. Cart Order Subtotal/Total updates to reflect only Product B. <br> 5. A success message (e.g., "[Product A] was removed from your shopping cart.") might appear, possibly with an "Undo" link. |                                  |                           |                          |
