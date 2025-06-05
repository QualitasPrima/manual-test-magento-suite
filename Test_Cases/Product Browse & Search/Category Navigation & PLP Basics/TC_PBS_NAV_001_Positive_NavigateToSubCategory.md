# Test Case: TC_PBS_NAV_001 - Navigation - Navigate to Sub-Category and Verify Products

* **Module:** Product Browse & Search
* **Feature:** Category Navigation
* **Objective:** Verify successful navigation to a product sub-category via the top menu, and that the PLP displays relevant products with correct breadcrumbs.
* **Priority:** Critical

**Preconditions:**
1.  User is on the Luma homepage.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Hover over a main category (e.g., "Women").                                           | Main Category: "Women"                        | Sub-menu for "Women" appears.                                                                                                                 |                                  |                           |                          |
| 2      | From the sub-menu, click on a sub-category (e.g., "Tops").                            | Sub-Category: "Tops"                          | User is redirected to the PLP for "Women > Tops".                                                                                             |                                  |                           |                          |
| 3      | Observe the PLP.                                                                      | -                                             | 1. Page title/heading indicates "Tops". <br> 2. Breadcrumbs show path like "Home > Women > Tops". <br> 3. Relevant products are displayed. |                                  |                           |                          |
