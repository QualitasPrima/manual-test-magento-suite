# Test Case: TC_PBS_FILTER_003 - Filtering - Apply Filters Resulting in No Products

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify an appropriate message is displayed when applied filters result in no matching products.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Apply a filter combination known/likely to yield no products.                         | e.g., Price $0.00-$0.01 or very specific unique combo | Filters applied.                                                                                                                              |                                  |                           |                          |
| 2      | Observe the product display area.                                                     | -                                             | No products displayed. Message "We can't find products matching the selection." (or similar) is shown. Active filters are still indicated.   |                                  |                           |                          |
