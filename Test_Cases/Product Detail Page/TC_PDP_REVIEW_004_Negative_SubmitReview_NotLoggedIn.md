# Test Case: TC_PDP_REVIEW_004 - Reviews - Attempt to Submit Review When Not Logged In

* **Module:** Product Detail Page
* **Feature:** Product Reviews
* **Objective:** Verify that a user who is not logged in is prompted to log in or cannot submit a review.
* **Priority:** Medium

**Preconditions:**
1.  User is NOT logged in.
2.  User is on the PDP of any product.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Reviews" tab on the PDP.                                             | -                                             | Review section loads.                                                                                                                         |                                  |                           |                          |
| 2      | Observe the review submission area/form.                                              | -                                             | Behavior depends on implementation: <br> 1. A message "Only registered users can write reviews. Please Sign in or create an account" is displayed, and the form might be hidden or disabled. <br> OR <br> 2. The form might be visible, but attempting to submit prompts for login. |                                  |                           |                          |
| 3      | If form is visible, attempt to fill it and click "Submit Review".                     | -                                             | User is redirected to the login page, or an inline login prompt appears. The review is not submitted without authentication.                 |                                  |                           |                          |
