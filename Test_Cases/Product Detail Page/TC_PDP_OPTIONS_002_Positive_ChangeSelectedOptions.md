# Test Case: TC_PDP_OPTIONS_002 - Options - Change Previously Selected Options

* **Module:** Product Detail Page
* **Feature:** Product Options Selection
* **Objective:** Verify that a user can change their previously selected size and color options to other valid options.
* **Priority:** High

**Preconditions:**
1.  User is on the PDP of a configurable product (e.g., "Radiant Tee").
2.  Valid size (e.g., "M") and color (e.g., "Orange") options have already been selected.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Initial selection: Size "M", Color "Orange".                                          | -                                             | "M" and "Orange" swatches are active/selected.                                                                                                |                                  |                           |                          |
| 2      | Click on a different available size swatch (e.g., "L").                               | New Size: "L"                                 | 1. The "L" size swatch becomes selected/highlighted. <br> 2. The "M" swatch is deselected. <br> 3. Color "Orange" remains selected.            |                                  |                           |                          |
| 3      | Click on a different available color swatch (e.g., "Blue").                           | New Color: "Blue"                             | 1. The "Blue" color swatch becomes selected/highlighted. <br> 2. The "Orange" swatch is deselected. <br> 3. Size "L" remains selected. <br> 4. Product image updates to "Blue" variant. |                                  |                           |                          |
