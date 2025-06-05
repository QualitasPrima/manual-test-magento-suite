# Test Case: TC_PBS_PLP_003 - PLP Basics - View/Items Per Page Controls on "No Results" Page

* **Module:** Product Browse & Search
* **Feature:** Product Listing Page (PLP) Display Options
* **Objective:** Verify the behavior and state of PLP view mode and "items per page" controls when a filter results in "no products found."
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP.
2.  User has applied filters such that the "We can't find products matching the selection." message is displayed (as in `TC_PBS_FILTER_003_Negative_FilterResultsInNoProducts.md`).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | After filtering to a "no products found" state, observe the view mode controls (Grid/List). | -                                             | View mode controls might be: <br> 1. Disabled or hidden (as there's nothing to change the view of). <br> OR <br> 2. Remain active but have no visual effect when clicked. (Observe actual Luma behavior). |                                  |                           |                          |
| 2      | Observe the "Show [Number] per page" or items per page selector.                      | -                                             | Items per page selector might be: <br> 1. Disabled or hidden. <br> OR <br> 2. Remain active but changing the value has no effect as there are no items. (Observe actual Luma behavior). |                                  |                           |                          |
| 3      | If controls are active, attempt to click/change them.                                 | -                                             | No errors occur. The "no products found" message persists. Controls do not cause unexpected behavior.                                         |                                  |                           |                          |
