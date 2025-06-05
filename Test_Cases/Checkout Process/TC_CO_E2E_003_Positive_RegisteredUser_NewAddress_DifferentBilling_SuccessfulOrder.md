# Test Case: TC_CO_E2E_003 - E2E - Registered User, New Shipping, Different New Billing

* **Module:** Checkout Process
* **Feature:** End-to-End Registered User Checkout
* **Objective:** Verify a registered user can complete checkout using a new shipping address and a new, different billing address.
* **Priority:** High

**Preconditions:**
1.  User is logged in.
2.  Shopping cart contains at least one item.
3.  User proceeds to checkout.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | On Shipping Address step, click "+ New Address" and fill in all mandatory new shipping address fields. | Valid new shipping details                    | New shipping address accepted.                                                                                                                |                                  |                           |                          |
| 2      | Select Shipping Method and click "Next".                                              | -                                             | Navigated to "Review & Payments".                                                                                                             |                                  |                           |                          |
| 3      | On "Review & Payments", verify Order Summary. Uncheck "My billing and shipping address are the same." | -                                             | Billing address form appears, or option to add new billing address.                                                                           |                                  |                           |                          |
| 4      | Select/Enter a new billing address different from the shipping address, filling all mandatory fields. | Valid new, different billing details          | New billing address accepted.                                                                                                                 |                                  |                           |                          |
| 5      | Click "Update" or similar if present for billing address. Select payment method.      | Payment Method: Check / Money order           | Payment method selected.                                                                                                                      |                                  |                           |                          |
| 6      | Click "Place Order".                                                                  | -                                             | Order placed successfully. User sees Order Confirmation. Both shipping and billing addresses used should be reflected if order details are checked. |                                  |                           |                          |
