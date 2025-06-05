# Test Case: TC_SC_VIEW_002 - View Cart - With Multiple Different Items

* **Module:** Shopping Cart
* **Feature:** View Cart Contents
* **Objective:** Verify that multiple, different products added to the cart are all listed correctly with their respective details.
* **Priority:** Critical

**Preconditions:**
1.  User has added at least two different products to the cart (e.g., Product A: "Radiant Tee", Qty 1; Product B: "Joust Duffle Bag", Qty 2).
2.  User navigates to the Shopping Cart page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the list of items in the cart.                                                | -                                             | Both Product A and Product B are listed as separate line items.                                                                               |                                  |                           |                          |
| 2      | For each product, verify its name, unit price, quantity, and item subtotal.           | -                                             | All details (name, price, quantity, options if any, subtotal) are correctly displayed for each individual product in the cart.              |                                  |                           |                          |
| 3      | Verify the overall cart summary (Order Subtotal).                                     | -                                             | The Order Subtotal in the cart summary correctly reflects the sum of all item subtotals.                                                      |                                  |                           |                          |
