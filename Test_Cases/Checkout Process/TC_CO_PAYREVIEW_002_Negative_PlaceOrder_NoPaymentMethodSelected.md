# Test Case: TC_CO_PAYREVIEW_002 - Payment & Review - Attempt to Place Order with No Payment Method Selected

* **Module:** Checkout Process
* **Feature:** Payment Method Selection
* **Objective:** Verify that the system prevents order placement if no payment method is selected (if UI allows such a state).
* **Priority:** High

**Preconditions:**
1.  User is on the "Review & Payments" step.
2.  Assume payment methods are radio buttons and none are selected by default (Luma usually has one pre-selected).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | If possible, ensure no payment method is selected.                                    | -                                             | No payment method is active.                                                                                                                  |                                  |                           |                          |
| 2      | Click "Place Order".                                                                  | -                                             | 1. Order is not placed. <br> 2. An error message "Please select a payment method." or similar is displayed. <br> (Note: Luma usually pre-selects "Check / Money order" if available, making this specific scenario hard to achieve without altering default behavior or having multiple unselected options). |                                  |                           |                          |
