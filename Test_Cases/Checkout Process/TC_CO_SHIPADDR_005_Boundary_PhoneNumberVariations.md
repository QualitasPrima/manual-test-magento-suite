# Test Case: TC_CO_SHIPADDR_005 - Shipping Address - Phone Number Field Variations

* **Module:** Checkout Process
* **Feature:** Shipping Address Validation
* **Objective:** Test the Phone Number field with various valid and just-out-of-boundary invalid formats (if specific formatting is expected/enforced).
* **Priority:** Medium

**Preconditions:**
1.  User is on the Shipping Address step, adding a new address.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Enter a phone number with too few digits. Fill other fields. Click "Next".            | Phone: `12345`                                | Error message for phone number format/length, or progression blocked.                                                                         |                                  |                           |                          |
| 2      | Enter a phone number with too many digits. Fill other fields. Click "Next".           | Phone: `1234567890123456`                     | Error message for phone number format/length, or progression blocked. Field might truncate input.                                             |                                  |                           |                          |
| 3      | Enter a phone number with letters. Fill other fields. Click "Next".                   | Phone: `123-ABC-DEFG`                         | Error message for phone number format (should be numeric), or progression blocked.                                                            |                                  |                           |                          |
| 4      | Enter a valid phone number format (e.g., 10 digits for US). Fill other fields. Click "Next". | Phone: `5551234567`                           | Input accepted, user proceeds to next step (assuming all other fields are valid).                                                             |                                  |                           |                          |
