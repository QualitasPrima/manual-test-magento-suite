# Test Case: TC_PBS_CATNAV_003 - Category Navigation - Attempt to Navigate to an Invalid/Non-Existent Category URL

* **Module:** Product Browse & Search
* **Feature:** Category Navigation
* **Objective:** Verify that the system handles attempts to navigate to a non-existent or invalid category URL gracefully (e.g., displays a "404 Not Found" page or a relevant error message).
* **Priority:** Medium

**Preconditions:**
1.  User has access to a browser and the base URL of the website.
2.  A known valid category URL structure (e.g., `.../women/tops-women.html`).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | In the browser's address bar, manually construct and attempt to navigate to a URL that points to a plausible but non-existent category path. | e.g., `https://magento.softwaretestingboard.com/non-existent-category.html` or `.../men/non-existent-subcategory.html` | URL is entered, navigation is attempted.                                                                                                      |                                  |                           |                          |
| 2      | Observe the page loaded.                                                              | -                                             | 1. The system does not crash or show a server error. <br> 2. A user-friendly "404 Page Not Found" page is displayed. <br> OR <br> 3. User is redirected to the homepage or a category landing page with a message like "Category not found." (Luma shows a "Whoops, our bad..." 404 page). |                                  |                           |                          |
