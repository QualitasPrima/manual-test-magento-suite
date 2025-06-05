# Test Case: TC_PBS_SORT_002 - Sorting - Sort Products by Price (Descending)

* **Module:** Product Browse & Search
* **Feature:** PLP Sorting
* **Objective:** Verify users can sort products by "Price" in descending order.
* **Priority:** High

**Preconditions:**
1.  User is on a PLP, products sorted by Price Ascending (from TC_PBS_SORT_001) or Price is selected in Sort By.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | "Price" is selected in "Sort By". Current order is Ascending.                         | -                                             | Prices are in ascending order.                                                                                                                |                                  |                           |                          |
| 2      | Click the sort direction icon/button (up/down arrow) to reverse the order.            | -                                             | PLP updates. Products are now sorted by price in descending order (High to Low). Verify prices are in descending order.                       |                                  |                           |                          |
