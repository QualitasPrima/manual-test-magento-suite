# Test Case: TC_CO_PAYREVIEW_001 - Payment & Review - Verify All Order Summary Details Before Placement

* **Module:** Checkout Process
* **Feature:** Order Review
* **Objective:** Verify that all order details (items, quantities, prices, selected shipping address, shipping method, totals) are accurately displayed on the Review & Payments page before placing the order.
* **Priority:** Critical

**Preconditions:**
1.  User has proceeded through shipping address and method selection.
2.  User is on the "Review & Payments" step.
3.  Cart contained specific items (e.g., Product A, Qty 2, Price $10; Product B, Qty 1, Price $25). Shipping Method chosen (e.g., Fixed Rate $5).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Carefully review the "Order Summary" section.                                         | -                                             | 1. Correct items (Product A, Product B) are listed with correct images and names. <br> 2. Correct quantities (A:2, B:1) are shown. <br> 3. Correct unit prices (A:$10, B:$25) and item subtotals (A:$20, B:$25) are shown. |                                  |                           |                          |
| 2      | Verify displayed Shipping Address.                                                    | -                                             | Matches the address entered/selected in the shipping step.                                                                                      |                                  |                           |                          |
| 3      | Verify displayed Shipping Method and its cost.                                        | -                                             | Matches method selected, and cost (e.g., $5) is correct.                                                                                        |                                  |                           |                          |
| 4      | Verify Subtotal, Shipping cost, and Order Total calculations.                         | Subtotal: $45, Shipping: $5                   | Subtotal = $45.00. Shipping = $5.00. Order Total = $50.00. All are correctly calculated and displayed.                                          |                                  |                           |                          |
