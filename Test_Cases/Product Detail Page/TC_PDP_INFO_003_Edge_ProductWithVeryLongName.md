# Test Case: TC_PDP_INFO_003 - Info - Product with Very Long Name Display

* **Module:** Product Detail Page
* **Feature:** Product Information Display
* **Objective:** Verify how the PDP layout handles a product with an exceptionally long name (checking for truncation, wrapping, or layout breaks).
* **Priority:** Low

**Preconditions:**
1.  A product with an unusually long name exists or can be simulated. (For Luma, may need to find one or assume one for conceptual testing).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the PDP of a product with a very long name.                               | Product: "This Is An Example Of A Product With An Extremely And Impractically Long Name To Test UI Layout" | PDP loads.                                                                                                                                    |                                  |                           |                          |
| 2      | Observe how the product name is displayed in the main title area.                     | -                                             | 1. The name is displayed. <br> 2. It either wraps gracefully to multiple lines. <br> OR <br> 3. It is truncated with an ellipsis (...) if it exceeds a certain display width. <br> 4. The overall page layout is not broken or distorted by the long name. |                                  |                           |                          |
| 3      | Check other areas where the name might appear (e.g., breadcrumbs, recently viewed - if applicable). | -                                             | Name is handled consistently and gracefully in other display areas.                                                                             |                                  |                           |                          |
