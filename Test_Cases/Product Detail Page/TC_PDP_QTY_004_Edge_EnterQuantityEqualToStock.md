# Test Case: TC_PDP_QTY_004 - Quantity - Enter Quantity Equal to Available Stock

* **Module:** Product Detail Page
* **Feature:** Quantity Input
* **Objective:** Verify ability to set quantity to the exact available stock amount (if stock is low and visible).
* **Priority:** Medium

**Preconditions:**
1.  User is on a PDP of a product with low, visible stock (e.g., "Only 5 left!"). This might need specific product setup or finding such a product. If not visible, this is harder to test precisely. Assume stock = 5 for this test.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the available stock mentioned as "5".                                         | Stock: 5                                      | Stock level is noted.                                                                                                                         |                                  |                           |                          |
| 2      | In the quantity field, enter the exact stock amount.                                  | Quantity: `5`                                 | The quantity "5" is accepted in the field.                                                                                                    |                                  |                           |                          |
| 3      | Click "Add to Cart".                                                                  | -                                             | Product with quantity 5 is successfully added to the cart. (Further checks on stock update are for cart/checkout tests).                      |                                  |                           |                          |
