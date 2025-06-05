# Test Case: TC_PDP_CART_002 - Add to Cart - Configurable Product with Selected Options and Quantity

* **Module:** Product Detail Page
* **Feature:** Add to Cart
* **Objective:** Verify that a configurable product can be added to the cart after selecting valid options and specifying a quantity.
* **Priority:** Critical

**Preconditions:**
1.  User is on the PDP of an in-stock configurable product (e.g., "Radiant Tee").

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Select a valid size option (e.g., "M").                                               | Size: "M"                                     | "M" size is selected.                                                                                                                         |                                  |                           |                          |
| 2      | Select a valid color option (e.g., "Blue").                                           | Color: "Blue"                                 | "Blue" color is selected. Product image may update.                                                                                           |                                  |                           |                          |
| 3      | Set the quantity to a valid number (e.g., "2").                                       | Quantity: 2                                   | Quantity field shows "2".                                                                                                                     |                                  |                           |                          |
| 4      | Click the "Add to Cart" button.                                                       | -                                             | 1. Success message displayed for adding "Radiant Tee" to cart. <br> 2. Mini-cart updates, reflecting 2 items of "Radiant Tee" with correct options. |                                  |                           |                          |
