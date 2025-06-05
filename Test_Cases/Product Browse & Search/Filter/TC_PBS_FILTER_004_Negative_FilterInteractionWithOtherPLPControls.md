# Test Case: TC_PBS_FILTER_004 - Filtering - Interaction of Filters with Sorting/Pagination

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify that applying or clearing filters interacts correctly with existing sort orders and pagination, ensuring data consistency.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP with multiple pages of products.
2.  A sort order other than default has been applied (e.g., Price High to Low).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Apply a filter that significantly reduces the number of products (e.g., to a single page). | e.g., Filter by a specific rare Brand or Style | 1. PLP updates, showing fewer products matching the filter. <br> 2. The existing sort order (Price High to Low) is maintained for the filtered results. <br> 3. Pagination updates correctly (e.g., may now show only 1 page). |                                  |                           |                          |
| 2      | Navigate to what would have been page 2 (or last page) if the filter was not applied (if pagination still shows multiple pages due to a UI bug, otherwise this step is N/A). | -                                             | If pagination incorrectly allows navigation, ensure no errors or unexpected products are shown. Ideally, pagination is correctly updated.        |                                  |                           |                          |
| 3      | Clear the applied filter.                                                             | -                                             | 1. PLP reverts to showing all products for the category. <br> 2. The original sort order (Price High to Low) is still applied. <br> 3. Pagination is restored to its original state. |                                  |                           |                          |
