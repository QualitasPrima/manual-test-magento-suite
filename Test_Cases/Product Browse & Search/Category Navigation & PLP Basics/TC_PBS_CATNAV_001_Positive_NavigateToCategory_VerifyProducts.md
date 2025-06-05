# Test Case: TC_PBS_CATNAV_001 - Category Navigation - Navigate to Category and Verify Products

* **Module:** Product Browse & Search
* **Feature:** Category Navigation
* **Objective:** Verify that users can successfully navigate to a product category via the top navigation menu and that the Product Listing Page (PLP) displays relevant products.
* **Priority:** Critical

**Preconditions:**
1.  User is on the Luma homepage or any other page with the main navigation menu visible.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the Luma homepage.                                                        | URL: `https://magento.softwaretestingboard.com/`              | Luma homepage loads successfully with the top navigation menu visible.                                                                        |                                  |                           |                          |
| 2      | Hover over a main category in the top navigation menu (e.g., "Women").                | Category: "Women"                             | A sub-menu/dropdown appears showing sub-categories (e.g., "Tops", "Bottoms").                                                               |                                  |                           |                          |
| 3      | From the sub-menu, click on a specific sub-category (e.g., "Tops").                   | Sub-category: "Tops"                          | User is redirected to the Product Listing Page for "Women > Tops".                                                                              |                                  |                           |                          |
| 4      | Observe the Product Listing Page.                                                     | -                                             | 1. The page title or breadcrumbs indicate the correct category (e.g., "Tops"). <br> 2. Multiple products are displayed on the page. <br> 3. Each product typically shows an image, name, price, and options like "Add to Cart". |                                  |                           |                          |
