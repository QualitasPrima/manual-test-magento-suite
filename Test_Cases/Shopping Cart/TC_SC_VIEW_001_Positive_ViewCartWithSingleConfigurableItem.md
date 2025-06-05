# Test Case: TC_SC_VIEW_001 - View Cart - With Single Configurable Item and Options

* **Module:** Shopping Cart
* **Feature:** View Cart Contents
* **Objective:** Verify that a single configurable product added to the cart is displayed correctly with its name, price, quantity, selected options (e.g., size, color), image, and item subtotal.
* **Priority:** Critical

**Preconditions:**
1.  User has added one configurable product (e.g., "Radiant Tee", Size M, Color Blue, Qty 1) to the shopping cart from its PDP.
2.  User navigates to the Shopping Cart page (`checkout/cart/`).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the product details for the item in the cart.                                 | Product: "Radiant Tee"                        | 1. Product image is displayed. <br> 2. Product Name ("Radiant Tee") is correct. <br> 3. Selected Size ("M") is displayed. <br> 4. Selected Color ("Blue") is displayed. <br> 5. Unit Price is correct. <br> 6. Quantity field shows "1". <br> 7. Item Subtotal (Price x Qty) is correct. |                                  |                           |                          |
| 2      | Verify other elements like "Edit" and "Remove" item options are present for the item. | -                                             | "Edit" (or pencil icon) and "Remove" (or trash icon) options are visible for the cart item.                                                 |                                  |                           |                          |
