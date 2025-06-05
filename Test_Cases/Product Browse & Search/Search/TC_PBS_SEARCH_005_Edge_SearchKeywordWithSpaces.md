# Test Case: TC_PBS_SEARCH_005 - Search - Keyword with Leading/Trailing Spaces

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify if search trims leading/trailing spaces from search terms.
* **Priority:** Medium

**Preconditions:**
1.  Product "Radiant Tee" exists.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "  Radiant Tee  " (with spaces) into search bar.                                 | Search Term: "  Radiant Tee  "                 | Text with spaces entered.                                                                                                                     |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | Ideally, spaces are trimmed, "Radiant Tee" product is found. (Observe if trimming occurs or if it leads to "no results").                      |                                  |                           |                          |
