# Test Case: TC_PBS_PLPVIEW_001 - PLP View - Change Product Display View Mode

* **Module:** Product Browse & Search
* **Feature:** PLP Display Options
* **Objective:** Verify that users can switch between "Grid" and "List" view modes on the PLP.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP with multiple products (e.g., "Women > Tops"). Default view is "Grid".

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Locate the view mode switcher (Grid/List icons/links).                                | -                                             | Switcher is visible. "Grid" is active.                                                                                                        |                                  |                           |                          |
| 2      | Click on the "List" view mode.                                                        | -                                             | PLP updates, products display in list format. "List" view is now active.                                                                      |                                  |                           |                          |
| 3      | Click back on the "Grid" view mode.                                                   | -                                             | PLP updates, products display in grid format. "Grid" view is now active.                                                                      |                                  |                           |                          |
