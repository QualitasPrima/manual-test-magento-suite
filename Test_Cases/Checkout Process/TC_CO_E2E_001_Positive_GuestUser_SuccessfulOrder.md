# Test Case: TC_CO_E2E_001 - E2E - Guest User Successful Order Placement

* **Module:** Checkout Process
* **Feature:** End-to-End Guest Checkout
* **Objective:** Verify that a guest user can successfully complete the checkout process by providing new shipping/billing information and placing an order.
* **Priority:** Critical

**Preconditions:**
1.  User is not logged in (guest user).
2.  Shopping cart contains at least one item.
3.  User has navigated from the Shopping Cart page by clicking "Proceed to Checkout".

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | On the Shipping Address step, enter a valid email address.                            | Email: `guest[timestamp]@example.com`          | Email entered.                                                                                                                                |                                  |                           |                          |
| 2      | Fill in all mandatory shipping address fields (First Name, Last Name, Street, City, State/Province, Zip, Country, Phone). | Valid shipping details                        | All mandatory shipping address fields are completed.                                                                                          |                                  |                           |                          |
| 3      | Select a Shipping Method (e.g., "Fixed - Flat Rate" is often default/only on Luma).   | -                                             | Shipping method is selected (or pre-selected). Shipping cost is displayed.                                                                    |                                  |                           |                          |
| 4      | Click "Next".                                                                         | -                                             | User is navigated to the "Review & Payments" step.                                                                                            |                                  |                           |                          |
| 5      | On the "Review & Payments" step, verify the Order Summary (items, prices, totals, shipping address, shipping method). | -                                             | All details in the Order Summary are correct and match previous selections/cart state.                                                        |                                  |                           |                          |
| 6      | Ensure "My billing and shipping address are the same" is checked (or uncheck and provide valid billing if testing that). | -                                             | Billing address configuration is set.                                                                                                         |                                  |                           |                          |
| 7      | Select a payment method (e.g., "Check / Money order").                                | Payment Method: Check / Money order           | Payment method is selected.                                                                                                                   |                                  |                           |                          |
| 8      | Click the "Place Order" button.                                                       | -                                             | 1. Order is successfully placed. <br> 2. User is redirected to the Order Success/Confirmation page. <br> 3. A "Thank you for your purchase!" message and an Order Number are displayed. |                                  |                           |                          |
