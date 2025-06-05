# Test Case: TC_PDP_OPTIONS_004 - Options - Interaction with Out-of-Stock Option Combinations

* **Module:** Product Detail Page
* **Feature:** Product Options Selection
* **Objective:** Verify how the UI indicates or handles option combinations that are out of stock.
* **Priority:** Medium

**Preconditions:**
1.  User is on the PDP of a configurable product.
2.  Assume a specific combination of options (e.g., Size "XL", Color "Purple" for "Radiant Tee") is out of stock. (This may require data setup or finding such a product if available on the demo site).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Select an option for the first attribute (e.g., Size "XL").                           | Size: "XL"                                    | "XL" is selected.                                                                                                                             |                                  |                           |                          |
| 2      | Observe the swatches for the second attribute (e.g., Color).                          | -                                             | The swatch for the out-of-stock color option ("Purple") when "XL" is selected should be: <br> 1. Visually distinct (e.g., grayed out, crossed out). <br> AND/OR <br> 2. Unselectable. |                                  |                           |                          |
| 3      | Attempt to select the out-of-stock option combination (e.g., "Purple" color swatch).  | Color: "Purple" (the out-of-stock one)      | Selection is prevented. The swatch is not highlighted as active. No error message is strictly necessary if selection is visually blocked.      |                                  |                           |                          |
| 4      | If selection was somehow possible, or if options update availability status AFTER selection, check "Add to Cart" button and stock status. | -                                             | "Add to Cart" button should be disabled, and/or an "Out of stock" message should appear for that specific combination.                       |                                  |                           |                          |
