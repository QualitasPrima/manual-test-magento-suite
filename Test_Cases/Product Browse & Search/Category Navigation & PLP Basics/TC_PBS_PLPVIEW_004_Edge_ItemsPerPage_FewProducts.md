# Test Case: TC_PBS_PLPVIEW_004 - PLP View - Items Per Page with Fewer Products than Selector Option

* **Module:** Product Browse & Search
* **Feature:** PLP Display Options
* **Objective:** Verify "items per page" behavior when a category has fewer products than the selected/lowest "items per page" option.
* **Priority:** Low

**Preconditions:**
1.  User is on a PLP for a category with a small number of products (e.g., 3 products). "Items per page" options are 12, 24, etc.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | On PLP with 3 products, select "12" (or lowest option > 3) from "items per page".     | Items per page: 12                            | All 3 available products are displayed. No errors. Pagination should not be visible.                                                          |                                  |                           |                          |
| 2      | Select a higher option, e.g., "24", from "items per page".                            | Items per page: 24                            | All 3 available products remain displayed. No errors.                                                                                           |                                  |                           |                          |
