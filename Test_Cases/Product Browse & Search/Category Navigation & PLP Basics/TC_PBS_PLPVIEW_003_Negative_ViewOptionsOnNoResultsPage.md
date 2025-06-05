# Test Case: TC_PBS_PLPVIEW_003 - PLP View - View/Items Per Page Controls on "No Results" Page

* **Module:** Product Browse & Search
* **Feature:** PLP Display Options
* **Objective:** Verify the behavior of PLP view mode and "items per page" controls when filters result in "no products found."
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP and has applied filters resulting in the "We can't find products matching the selection." message.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | With "no products found" message visible, observe view mode controls (Grid/List).     | -                                             | Controls might be disabled/hidden or remain active but have no effect. No errors occur.                                                         |                                  |                           |                          |
| 2      | Observe the "Show [Number] per page" selector.                                        | -                                             | Selector might be disabled/hidden or remain active but have no effect. No errors occur.                                                         |                                  |                           |                          |
