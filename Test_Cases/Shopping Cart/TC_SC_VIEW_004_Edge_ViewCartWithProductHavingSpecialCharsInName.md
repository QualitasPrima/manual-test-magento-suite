# Test Case: TC_SC_VIEW_004 - View Cart - With Product Having Special Characters in Name/Options

* **Module:** Shopping Cart
* **Feature:** View Cart Contents
* **Objective:** Verify that product names and selected options containing special characters (e.g., accents, symbols if allowed) are displayed correctly in the cart.
* **Priority:** Low

**Preconditions:**
1.  A product exists whose name or selectable option values contain special characters (e.g., "Café Thermos" or Size "S/M"). (This may require data setup or finding such a product).
2.  User has added this product to the cart and navigates to the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the product details in the cart, focusing on the name and any selected options. | Product with special chars in name/option   | The product name and/or options are displayed correctly, with special characters rendered accurately (not garbled, escaped, or causing display issues). |                                  |                           |                          |
