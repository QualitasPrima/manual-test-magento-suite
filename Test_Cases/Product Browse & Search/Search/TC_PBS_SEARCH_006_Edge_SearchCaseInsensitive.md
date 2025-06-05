# Test Case: TC_PBS_SEARCH_006 - Search - Case Insensitivity Check

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify search is case-insensitive for product names/keywords.
* **Priority:** High

**Preconditions:**
1.  Product "Radiant Tee" exists.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "rAdIaNt TeE" into search bar.                                                   | Search Term: "rAdIaNt TeE"                    | Mixed case text entered.                                                                                                                      |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | "Radiant Tee" product is displayed, indicating case-insensitive search.                                                                         |                                  |                           |                          |
