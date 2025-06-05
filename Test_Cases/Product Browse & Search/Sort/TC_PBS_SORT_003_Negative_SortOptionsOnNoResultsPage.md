# Test Case: TC_PBS_SORT_003 - Sorting - Sort Options on "No Results" Page

* **Module:** Product Browse & Search
* **Feature:** PLP Sorting
* **Objective:** Verify the behavior of sort controls when filters result in "no products found."
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP and has applied filters resulting in the "We can't find products matching the selection." message.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | With "no products found" message visible, observe the "Sort By" control.              | -                                             | "Sort By" control might be: <br> 1. Disabled or hidden. <br> OR <br> 2. Remain active but changing selection has no effect. No errors occur. |                                  |                           |                          |
