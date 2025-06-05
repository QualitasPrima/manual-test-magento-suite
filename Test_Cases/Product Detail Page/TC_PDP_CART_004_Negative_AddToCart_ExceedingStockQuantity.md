# Test Case: TC_PDP_CART_004 - Add to Cart - Attempt to Add Quantity Exceeding Available Stock

* **Module:** Product Detail Page
* **Feature:** Add to Cart / Quantity Input
* **Objective:** Verify system behavior when user tries to add a quantity greater than the available stock.
* **Priority:** High

**Preconditions:**
1.  User is on PDP of a product with limited, known stock (e.g., 5 items available). Stock visibility is helpful.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Assume available stock is 5. In quantity field, enter a number greater than stock.    | Quantity: `10` (Stock is 5)                   | Quantity "10" is entered.                                                                                                                     |                                  |                           |                          |
| 2      | Click "Add to Cart".                                                                  | -                                             | Behavior depends on implementation: <br> 1. An error message is displayed indicating requested quantity exceeds stock, product not added or only available stock added. <br> OR <br> 2. Quantity field auto-corrects to max available stock before adding. (Luma usually shows error: "The requested qty is not available"). |                                  |                           |                          |
