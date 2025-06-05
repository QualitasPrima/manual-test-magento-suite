# Test Case: TC_SC_REMOVE_003 - Remove Item - Verify "Undo" Functionality After Item Removal

* **Module:** Shopping Cart
* **Feature:** Remove Item (Undo)
* **Objective:** Verify that if an "Undo" option is provided after removing an item, using it restores the item to the cart correctly. (Luma shows an "Undo" link in the success message for a short time).
* **Priority:** Medium

**Preconditions:**
1.  Cart contains at least one item (Product A). User is on the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Click the "Remove" icon/link for Product A.                                           | Remove Product A                              | Product A is removed. A success message appears, containing an "Undo" link (e.g., "ITEM_NAME was removed from your shopping cart. Undo").     |                                  |                           |                          |
| 2      | Quickly click the "Undo" link within the success message before it disappears.        | Click "Undo"                                  | 1. Product A is restored to the shopping cart with its original quantity and options. <br> 2. Cart totals are updated to reflect the restored item. <br> 3. The success message (and Undo link) for removal disappears. |                                  |                           |                          |
| 3      | If "Undo" link is not clicked and message times out/user navigates away and back, verify item is permanently removed. | -                                             | Product A remains removed from the cart.                                                                                                      |                                  |                           |                          |
