# Test Case: TC_CO_PAYREVIEW_004 - Payment & Review - Place Order with $0.00 Order Total

* **Module:** Checkout Process
* **Feature:** Place Order
* **Objective:** Verify that an order with a $0.00 total (e.g., due to 100% discount) can be successfully placed and how payment methods are handled.
* **Priority:** Medium

**Preconditions:**
1.  Cart contains item(s) resulting in an Order Total of $0.00 after discounts.
2.  User is on the "Review & Payments" step.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Verify Order Total is $0.00.                                                          | -                                             | Order Total is $0.00.                                                                                                                         |                                  |                           |                          |
| 2      | Observe Payment Method section.                                                       | -                                             | Payment methods might be: <br> 1. Still selectable (e.g., "Check / Money order" or a "No Payment Information Required" option might appear). <br> OR <br> 2. Section might be bypassed or hidden. |                                  |                           |                          |
| 3      | Select a payment method if required/available (e.g., "No Payment Information Required" or "Check/Money order" if it allows $0). | -                                             | Method selected if applicable.                                                                                                                |                                  |                           |                          |
| 4      | Click "Place Order".                                                                  | -                                             | Order is placed successfully. User is taken to Order Confirmation page. No actual payment transaction should be attempted if total is $0.00.     |                                  |                           |                          |
