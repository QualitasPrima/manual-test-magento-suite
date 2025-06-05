# Test Case: TC_PBS_FILTER_005 - Filtering - Price Range Filter with Exact Boundary Values

* **Module:** Product Browse & Search
* **Feature:** PLP Filtering
* **Objective:** Verify correct product display when filtering by a price range using exact boundary values (min and max of the range slider/inputs).
* **Priority:** Medium

**Preconditions:**
1.  User is on a PLP with a price range filter available.
2.  There are products with prices at or near the typical min/max ends of the filterable range.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Observe the available price range in the filter (e.g., $10.00 - $100.00).             | -                                             | Price range is visible.                                                                                                                       |                                  |                           |                          |
| 2      | Adjust the price filter to select only the minimum possible range allowed by the slider/inputs (e.g., if slider allows selecting $10.00-$10.00 or $10.00-$11.00). | Min Price: e.g., $10.00, Max Price: e.g., $10.99 (or smallest range possible) | 1. PLP updates. <br> 2. Only products falling exactly within this very narrow selected price range are displayed. <br> 3. Inclusivity of boundaries (e.g. >= min AND <= max) is verified. |                                  |                           |                          |
| 3      | Adjust the price filter to select only the maximum possible range allowed by the slider/inputs (e.g., $99.00-$100.00). | Min Price: e.g., $99.00, Max Price: e.g., $100.00 | 1. PLP updates. <br> 2. Only products falling exactly within this narrow high-end selected price range are displayed.                          |                                  |                           |                          |
| 4      | Adjust the filter to cover the entire available price range.                          | Min Price: e.g., $10.00, Max Price: e.g., $100.00 | PLP updates. All products within the overall min/max price points for the category are displayed (effectively no price filtering if it's the full range). |                                  |                           |                          |
