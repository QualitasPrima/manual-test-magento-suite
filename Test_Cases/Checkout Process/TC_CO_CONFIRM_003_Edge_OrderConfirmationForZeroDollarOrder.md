# Test Case: TC_CO_CONFIRM_003 - Order Confirmation - Display for a $0.00 Order

* **Module:** Checkout Process
* **Feature:** Order Confirmation
* **Objective:** Verify that the order confirmation page for a $0.00 order (e.g., fully discounted item) displays appropriate messaging and order details.
* **Priority:** Medium

**Preconditions:**
1.  User has successfully placed an order where the final Order Total was $0.00.
2.  User is on the Order Success/Confirmation page.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the content of the Order Confirmation page, especially any payment-related info. | -                                             | 1. Standard success message and Order ID are displayed. <br> 2. Order summary correctly shows items and $0.00 total. <br> 3. Any payment information section should reflect that no payment was processed or needed (e.g., "No payment information required" or similar, or simply omits payment details). |                                  |                           |                          |
