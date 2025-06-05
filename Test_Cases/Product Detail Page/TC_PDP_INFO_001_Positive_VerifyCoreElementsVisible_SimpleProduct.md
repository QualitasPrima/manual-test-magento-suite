# Test Case: TC_PDP_INFO_001 - Info - Verify Core Elements Visible (Simple Product)

* **Module:** Product Detail Page
* **Feature:** Product Information Display
* **Objective:** Verify that all essential product information elements (name, price, image, SKU, description, Add to Cart button) are visible and correctly displayed for a simple product.
* **Priority:** Critical

**Preconditions:**
1.  User has navigated to the PDP of a simple product (e.g., "Push It Messenger Bag" - which doesn't require size/color options).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the main content area of the PDP.                                             | Product: e.g., "Push It Messenger Bag"        | 1. Product Name is prominently displayed and matches the product. <br> 2. Product Price is clearly visible and correctly formatted. <br> 3. Main Product Image is displayed. <br> 4. Product SKU is visible. <br> 5. "Add to Cart" button is visible and enabled (if in stock). <br> 6. Stock status (e.g., "In Stock") is visible. <br> 7. Short description (if any) is visible. |                                  |                           |                          |
| 2      | Scroll down to view tabs like "Details", "More Information", "Reviews".               | -                                             | Tabs are visible. "Details" tab typically shows the longer product description. "More Information" shows attributes like style, material etc. |                                  |                           |                          |
| 3      | Click on the "More Information" tab.                                                  | -                                             | The "More Information" tab content is displayed, showing relevant product attributes and their values.                                          |                                  |                           |                          |
