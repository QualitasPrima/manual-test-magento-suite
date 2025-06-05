# Test Case: TC_PBS_PLPVIEW_002 - PLP View - Change Number of Items Displayed Per Page

* **Module:** Product Browse & Search
* **Feature:** PLP Display Options
* **Objective:** Verify that users can change the number of products displayed per page on the PLP.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP with more products than the default "items per page" setting (e.g., a category with 30 products, default showing 12).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Locate the "Show [Number] per page" selector. Note the current value.                 | -                                             | Selector is visible.                                                                                                                          |                                  |                           |                          |
| 2      | Select a different, higher number of items per page (e.g., 24, if available).         | New items per page: e.g., 24                  | PLP reloads/updates. The number of products displayed changes to the new selection (or max available if less than selection).                   |                                  |                           |                          |
| 3      | Select a different, lower number of items per page (e.g., 12).                        | New items per page: e.g., 12                  | PLP reloads/updates. The number of products displayed changes to the new selection.                                                             |                                  |                           |                          |
