# Test Case: TC_PBS_FILTER_001 - Filtering - Filter by a Single Attribute (e.g., Color)

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify successful product filtering using a single attribute, displaying only matching products.
* **Priority:** High

**Preconditions:**
1.  User is on a PLP with filterable attributes (e.g., "Men > Tops").

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In filter options, select a value for an attribute (e.g., "COLOR": "Blue").           | Attribute: COLOR, Value: Blue                 | PLP updates. Selected filter ("Blue") is active. All displayed products are blue.                                                             |                                  |                           |                          |
| 2      | Clear the applied filter.                                                             | -                                             | PLP updates. Filter is removed. Product list reverts to pre-filter state.                                                                       |                                  |                           |                          |
