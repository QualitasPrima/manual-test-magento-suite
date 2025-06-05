# Test Case: TC_PBS_NAV_002 - Navigation - Attempt to Navigate to an Invalid Category URL

* **Module:** Product Browse & Search
* **Feature:** Category Navigation
* **Objective:** Verify graceful handling of attempts to navigate to a non-existent category URL.
* **Priority:** Medium

**Preconditions:**
1.  Base URL of the website is known.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Manually enter a URL for a non-existent category path in the browser address bar.     | e.g., `https://magento.softwaretestingboard.com/non-existent-category.html` | Navigation is attempted.                                                                                                                      |                                  |                           |                          |
| 2      | Observe the page loaded.                                                              | -                                             | A user-friendly "404 Page Not Found" (or similar error page like "Whoops, our bad...") is displayed. System does not crash.                 |                                  |                           |                          |
