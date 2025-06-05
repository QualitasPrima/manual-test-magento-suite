# Test Case: TC_CO_E2E_002 - E2E - Registered User with Saved Address Successful Order

* **Module:** Checkout Process
* **Feature:** End-to-End Registered User Checkout
* **Objective:** Verify that a logged-in registered user can successfully complete checkout using a saved shipping address.
* **Priority:** Critical

**Preconditions:**
1.  User is logged in and has at least one saved shipping address in their account.
2.  Shopping cart contains at least one item.
3.  User proceeds to checkout.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | On the Shipping Address step, a saved address is automatically selected, or user selects one from their address book. | -                                             | A valid saved shipping address is selected/displayed.                                                                                         |                                  |                           |                          |
| 2      | Select a Shipping Method.                                                             | -                                             | Shipping method selected. Shipping cost displayed.                                                                                            |                                  |                           |                          |
| 3      | Click "Next".                                                                         | -                                             | User navigated to "Review & Payments".                                                                                                        |                                  |                           |                          |
| 4      | Verify Order Summary and selected shipping address.                                   | -                                             | Details are correct.                                                                                                                          |                                  |                           |                          |
| 5      | Select payment method (e.g., "Check / Money order").                                  | Payment Method: Check / Money order           | Payment method selected.                                                                                                                      |                                  |                           |                          |
| 6      | Click "Place Order".                                                                  | -                                             | Order placed successfully. User sees Order Confirmation page with Order Number.                                                                 |                                  |                           |                          |
