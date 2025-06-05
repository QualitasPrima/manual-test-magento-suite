# Test Case: TC_PBS_FILTER_006 - Filtering - Select All Available Options for a Multi-Select Attribute

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify system behavior when all available options for a multi-select filter attribute (e.g., all available 'Colors' or 'Sizes') are selected.
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP with a filter attribute that allows multiple selections (e.g., "Color" where you can check Blue, Red, Green).
2.  The attribute has 2+ options.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Identify a multi-select filter attribute (e.g., "Color").                             | Attribute: Color                              | Filter options (e.g., Blue, Green, Red) are visible.                                                                                          |                                  |                           |                          |
| 2      | Select the first option (e.g., "Blue").                                               | Select "Blue"                                 | PLP updates, showing blue products. "Blue" is active.                                                                                         |                                  |                           |                          |
| 3      | Select the second available option for the same attribute (e.g., "Green") without deselecting the first. | Select "Green"                                | PLP updates. Products that are "Blue" OR "Green" are displayed. Both "Blue" and "Green" are shown as active filters. (Luma typically uses OR logic for multiple selections within the same attribute). |                                  |                           |                          |
| 4      | Continue selecting all available options for that attribute.                          | Select all available colors                     | PLP updates. All products that match any of the selected colors are displayed. Effectively, if all colors are selected, this might be similar to no color filter being applied (all products shown based on other filters). |                                  |                           |                          |
| 5      | Deselect one of the options.                                                          | Deselect "Blue"                               | PLP updates. Products matching the remaining selected colors (e.g., "Green" AND any other selected colors) are displayed.                     |                                  |                           |                          |
