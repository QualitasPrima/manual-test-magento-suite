# Test Case: TC_CO_PAYREVIEW_003 - Payment & Review - Different Billing Address with Missing Required Fields

* **Module:** Checkout Process
* **Feature:** Billing Address Validation
* **Objective:** Verify error handling if "Bill to this address" is different from shipping, and the new billing address form has missing mandatory fields when trying to place order.
* **Priority:** High

**Preconditions:**
1.  User is on "Review & Payments". Shipping address is valid.
2.  User has unchecked "My billing and shipping address are the same."
3.  The billing address form is displayed.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In the billing address form, fill some fields but leave a mandatory one empty (e.g., Billing Street Address). | Billing Street: (empty)                     | Billing Street Address is empty.                                                                                                              |                                  |                           |                          |
| 2      | Select a payment method. Click "Place Order" (or "Update" for address then "Place Order"). | -                                             | 1. Order is not placed. <br> 2. An error message "This is a required field." is displayed for the missing billing address field(s).             |                                  |                           |                          |
