# Test Case: TC_PDP_OPTIONS_003 - Options - Attempt Add to Cart Without Selecting Required Options

* **Module:** Product Detail Page
* **Feature:** Product Options Selection / Add to Cart
* **Objective:** Verify that the system prevents adding a configurable product to the cart if required options (e.g., size, color) are not selected, and provides appropriate feedback.
* **Priority:** Critical

**Preconditions:**
1.  User is on the PDP of a configurable product (e.g., "Radiant Tee") that requires size and color selection.
2.  No options are selected by default.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Do not select any size.                                                               | -                                             | No size is selected.                                                                                                                          |                                  |                           |                          |
| 2      | Do not select any color.                                                              | -                                             | No color is selected.                                                                                                                         |                                  |                           |                          |
| 3      | Click the "Add to Cart" button.                                                       | -                                             | 1. Product is NOT added to the cart. <br> 2. Error messages are displayed near the unselected options (e.g., "This is a required field." for Size and Color). <br> 3. (Alternatively) The "Add to Cart" button might be disabled until all required options are chosen. (Luma shows messages). |                                  |                           |                          |
| 4      | Select only Size (e.g., "M") but not Color. Click "Add to Cart".                      | Size: "M", No Color selected                  | Product is NOT added to the cart. Error message for Color is displayed.                                                                       |                                  |                           |                          |
