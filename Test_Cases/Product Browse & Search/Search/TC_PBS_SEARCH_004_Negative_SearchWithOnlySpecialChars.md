# Test Case: TC_PBS_SEARCH_004 - Search - Using Only Special Characters

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify system behavior for search using only special characters.
* **Priority:** Medium

**Preconditions:**
1.  None.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "!@#$%^" into search bar.                                                        | Search Term: "!@#$%^"                         | Text entered.                                                                                                                                 |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | "No results found" message, or search ignored. System handles gracefully without errors.                                                        |                                  |                           |                          |
