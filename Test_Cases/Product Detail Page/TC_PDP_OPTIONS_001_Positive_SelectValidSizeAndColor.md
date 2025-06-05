# Test Case: TC_PDP_OPTIONS_001 - Options - Select Valid Size and Color

* **Module:** Product Detail Page
* **Feature:** Product Options Selection
* **Objective:** Verify that a user can successfully select available size and color options for a configurable product.
* **Priority:** Critical

**Preconditions:**
1.  User is on the PDP of a configurable product (e.g., "Radiant Tee") that has size and color options.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the available size options (e.g., XS, S, M, L, XL swatches).                  | -                                             | Size options are visible. None are selected by default.                                                                                       |                                  |                           |                          |
| 2      | Click on a valid, available size swatch (e.g., "M").                                  | Size: "M"                                     | 1. The "M" size swatch is highlighted or indicated as selected. <br> 2. (If applicable) Price or availability information might update.         |                                  |                           |                          |
| 3      | Observe the available color options (e.g., Blue, Orange, Purple swatches).            | -                                             | Color options are visible.                                                                                                                    |                                  |                           |                          |
| 4      | Click on a valid, available color swatch (e.g., "Orange").                            | Color: "Orange"                               | 1. The "Orange" color swatch is highlighted or indicated as selected. <br> 2. (If applicable) The main product image updates to the orange variant. <br> 3. (If applicable) Price or availability might update. |                                  |                           |                          |
| 5      | Verify that the "Add to Cart" button is now enabled (if it was disabled before option selection). | -                                             | "Add to Cart" button is enabled.                                                                                                              |                                  |                           |                          |
