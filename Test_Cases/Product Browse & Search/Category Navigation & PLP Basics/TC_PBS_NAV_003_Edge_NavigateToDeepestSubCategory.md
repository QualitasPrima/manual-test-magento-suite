# Test Case: TC_PBS_NAV_003 - Navigation - Navigate to Deepest Available Sub-Category

* **Module:** Product Browse & Search
* **Feature:** Category Navigation
* **Objective:** Verify successful navigation and correct display for the most deeply nested available sub-category.
* **Priority:** Medium

**Preconditions:**
1.  User is on the Luma homepage. (Identify deepest path e.g., Men > Tops > Hoodies & Sweatshirts)

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate through the menu structure to the deepest identified sub-category.           | Path: e.g., Men > Tops > Hoodies & Sweatshirts | User successfully navigates to the PLP of the deepest sub-category.                                                                             |                                  |                           |                          |
| 2      | Observe the PLP.                                                                      | -                                             | 1. Breadcrumbs accurately reflect the full path. <br> 2. Page title matches the category. <br> 3. Relevant products (or "no products" message if empty but valid) are displayed. |                                  |                           |                          |
