# Test Case: TC_PBS_SEARCH_001 - Search - By Full Valid Product Name

* **Module:** Product Browse & Search
* **Feature:** Search Functionality
* **Objective:** Verify searching with a full, valid product name returns the correct product.
* **Priority:** Critical

**Preconditions:**
1.  Product "Radiant Tee" exists.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Type "Radiant Tee" into the search bar.                                               | Search Term: "Radiant Tee"                    | Text entered. Autocomplete may appear.                                                                                                        |                                  |                           |                          |
| 2      | Press Enter or click search icon.                                                     | -                                             | Search results page for "Radiant Tee" loads. "Radiant Tee" product is prominently displayed.                                                    |                                  |                           |                          |
