# Test Case: TC_PBS_SORT_001 - Sorting - Sort Products by Price (Ascending)

* **Module:** Product Browse & Search
* **Feature:** PLP Sorting
* **Objective:** Verify users can sort products by "Price" in ascending order.
* **Priority:** High

**Preconditions:**
1.  User is on a PLP with multiple products having different prices.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Locate "Sort By" selector.                                                            | -                                             | Selector visible.                                                                                                                             |                                  |                           |                          |
| 2      | Select "Price" from "Sort By".                                                        | Sort Option: Price                            | PLP updates. Products are sorted by price (typically ascending by default for first click on Luma). Verify prices are in ascending order.   |                                  |                           |                          |
