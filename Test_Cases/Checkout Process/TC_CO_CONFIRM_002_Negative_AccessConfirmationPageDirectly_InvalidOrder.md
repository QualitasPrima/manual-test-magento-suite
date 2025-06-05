# Test Case: TC_CO_CONFIRM_002 - Order Confirmation - Attempt Direct URL Access to Confirmation Page (Invalid Order)

* **Module:** Checkout Process
* **Feature:** Order Confirmation
* **Objective:** Verify system behavior when attempting to directly access an order success/confirmation page URL without a valid preceding order or with an invalid order ID.
* **Priority:** Medium

**Preconditions:**
1.  The URL pattern for the order success page is known (e.g., `.../checkout/onepage/success/` or with an order ID parameter).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In a new browser session or after logging out, attempt to navigate directly to the order success URL, possibly with a fake/old order ID if URL structure uses one. | URL: e.g., `.../checkout/onepage/success/`  | Navigation is attempted.                                                                                                                      |                                  |                           |                          |
| 2      | Observe the loaded page.                                                              | -                                             | 1. The system does not display a fake success message or details of an unrelated order. <br> 2. User is redirected to the homepage, login page, or an error page/empty cart page. <br> 3. No sensitive order information is exposed. |                                  |                           |                          |
