# Test Case: TC_PBS_SEARCH_003 - Search - Non-Existent Search Term

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify a "no results" message for terms not matching any products.
* **Priority:** High

**Preconditions:**
1.  None.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "qwertyasdfzxcvb" into search bar.                                               | Search Term: "qwertyasdfzxcvb"                | Text entered.                                                                                                                                 |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | Search results page loads. Message "Your search returned no results." (or similar) is displayed.                                                |                                  |                           |                          |
