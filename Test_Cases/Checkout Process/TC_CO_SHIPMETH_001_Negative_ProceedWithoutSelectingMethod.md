# Test Case: TC_CO_SHIPMETH_001 - Shipping Method - Proceed Without Selecting a Method

* **Module:** Checkout Process
* **Feature:** Shipping Method Selection
* **Objective:** Verify that if no shipping method is selected (and one is not pre-selected by default), the user cannot proceed, or an error is shown.
* **Priority:** Medium

**Preconditions:**
1.  User is on the Shipping Method selection step.
2.  Assume UI allows a state where no method is initially selected (less common on Luma where "Fixed" is usually auto-selected if it's the only option). If Luma always pre-selects, this tests trying to *de-select* and proceed.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | If multiple shipping methods exist and none are pre-selected, do not select any.      | -                                             | No method selected.                                                                                                                           |                                  |                           |                          |
| 2      | Click "Next".                                                                         | -                                             | 1. User is prevented from proceeding. <br> 2. An error message "Please select a shipping method." or similar is displayed. <br> (Note: Luma often has "Fixed" rate pre-selected if it's the only one, making this hard to test directly unless there are multiple options and no default.) |                                  |                           |                          |
