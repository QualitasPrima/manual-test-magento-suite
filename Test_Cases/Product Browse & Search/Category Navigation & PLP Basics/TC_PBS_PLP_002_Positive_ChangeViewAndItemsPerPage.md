# Test Case: TC_PBS_PLP_002 - PLP - Change Product View and Items Per Page

* **Module:** Product Browse & Search
* **Feature:** Product Listing Page (PLP) Display Options
* **Objective:** Verify that users can change the product display view (e.g., grid to list) and the number of items displayed per page on the PLP.
* **Priority:** Medium

**Preconditions:**
1.  User has navigated to a Product Listing Page with multiple products and display options available. (e.g., "Women > Tops").

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | On the PLP, locate the view mode switcher (e.g., "Grid" and "List" icons/links).      | -                                             | View mode switcher is visible. Assume "Grid" is the default active view.                                                                      |                                  |                           |                          |
| 2      | Click on the "List" view mode.                                                        | View Mode: "List"                             | 1. The PLP reloads or updates. <br> 2. Products are now displayed in a list format (typically one product per row with more details visible). <br> 3. The "List" view mode is indicated as active. |                                  |                           |                          |
| 3      | Locate the "Show [Number] per page" dropdown/selector (or similar for items per page). | -                                             | Items per page selector is visible. Note the current number of items displayed.                                                               |                                  |                           |                          |
| 4      | Select a different number of items per page from the selector (e.g., if current is 12, select 24, if available). | Items per page: e.g., 24                    | 1. The PLP reloads or updates. <br> 2. The number of products displayed on the page changes to the selected value (or up to the total number of products in the category if less than selected). |                                  |                           |                          |
| 5      | Click back to "Grid" view mode.                                                       | View Mode: "Grid"                             | Products are displayed in grid format again, respecting the new items per page setting.                                                         |                                  |                           |                          |
