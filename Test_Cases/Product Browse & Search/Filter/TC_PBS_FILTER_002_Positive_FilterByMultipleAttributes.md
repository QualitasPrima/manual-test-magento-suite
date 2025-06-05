# Test Case: TC_PBS_FILTER_002 - Filtering - Apply Multiple Different Filter Attributes

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify successful product filtering when multiple filters across different attributes are applied simultaneously.
* **Priority:** High

**Preconditions:**
1.  User is on a PLP (e.g., "Women > Tops > Jackets").

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Select a filter (e.g., "STYLE": "Jacket").                                            | STYLE: Jacket                                 | PLP updates, shows jackets.                                                                                                                   |                                  |                           |                          |
| 2      | Select another filter from a different attribute (e.g., "COLOR": "Black").            | COLOR: Black                                  | PLP updates, shows black jackets. Both filters are active.                                                                                    |                                  |                           |                          |
| 3      | Select a third filter (e.g., "SIZE": "M").                                            | SIZE: M                                       | PLP updates, shows black jackets of size M. All three filters are active. Displayed products match all criteria.                              |                                  |                           |                          |
