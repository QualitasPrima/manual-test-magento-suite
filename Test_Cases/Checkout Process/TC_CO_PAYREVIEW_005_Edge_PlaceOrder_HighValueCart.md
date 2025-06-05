# Test Case: TC_CO_PAYREVIEW_005 - Payment & Review - Place Order with High Value Cart

* **Module:** Checkout Process
* **Feature:** Place Order
* **Objective:** Verify successful order placement for a cart with a very high total value (testing for calculation/system limits, if any).
* **Priority:** Low

**Preconditions:**
1.  Cart contains items resulting in a very high Order Total (e.g., > $10,000 or maximum plausible). (Conceptual items may be needed).
2.  User is on the "Review & Payments" step.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Verify Order Total is a very large number, correctly calculated and formatted.        | -                                             | Order Total is correct.                                                                                                                       |                                  |                           |                          |
| 2      | Select payment method (e.g., "Check / Money order").                                  | -                                             | Payment method selected.                                                                                                                      |                                  |                           |                          |
| 3      | Click "Place Order".                                                                  | -                                             | Order is placed successfully without calculation errors or system timeouts related to the high value. User sees Order Confirmation page.          |                                  |                           |                          |
