# Test Case: TC_PBS_SEARCH_002 - Search - By Partial Keyword Yielding Multiple Results

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify searching with a common partial keyword returns multiple relevant products.
* **Priority:** High

**Preconditions:**
1.  Multiple products contain "Bag" or "Tank".

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "Bag" into the search bar.                                                       | Search Term: "Bag"                            | Text entered.                                                                                                                                 |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | Search results page for "Bag" loads. Multiple products relevant to "Bag" are displayed.                                                         |                                  |                           |                          |
