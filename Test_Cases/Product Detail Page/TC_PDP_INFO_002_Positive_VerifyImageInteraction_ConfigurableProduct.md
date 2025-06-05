# Test Case: TC_PDP_INFO_002 - Info - Verify Image Interaction (Configurable Product with Options)

* **Module:** Product Detail Page
* **Feature:** Product Information Display (Images)
* **Objective:** Verify image thumbnails, main image update on option selection (if applicable), and image zoom functionality for a configurable product.
* **Priority:** High

**Preconditions:**
1.  User has navigated to the PDP of a configurable product with multiple images and options that might change the image (e.g., "Radiant Tee" - different colors have different images).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the product image area.                                                       | Product: e.g., "Radiant Tee"                  | A main product image and several smaller thumbnail images (if available for the product/default option) are displayed.                        |                                  |                           |                          |
| 2      | Click on a different thumbnail image.                                                 | -                                             | The main product image updates to display the selected thumbnail image.                                                                       |                                  |                           |                          |
| 3      | Select a product option that is known to have a different image (e.g., a different color for "Radiant Tee"). | Option: e.g., Color Orange                      | The main product image updates to show the image associated with the selected color option. Thumbnail images might also update.             |                                  |                           |                          |
| 4      | Hover the mouse cursor over the main product image.                                   | -                                             | A zoomed-in view or lens effect appears over the image, allowing detailed inspection. (Or click to open full-size gallery).                  |                                  |                           |                          |
