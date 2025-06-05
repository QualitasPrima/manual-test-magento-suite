# Test Case: TC_PDP_REVIEW_005 - Reviews - Submit Review with Minimum and Maximum Star Rating

* **Module:** Product Detail Page
* **Feature:** Product Reviews
* **Objective:** Verify successful review submission using the minimum (1 star) and maximum (5 star) possible ratings.
* **Priority:** Medium

**Preconditions:**
1.  User is logged in and on the PDP "Reviews" tab.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Fill all required review fields (Nickname, Summary, Review). Select 1 star rating.    | Rating: 1 star                                | Review details entered, 1 star selected.                                                                                                      |                                  |                           |                          |
| 2      | Click "Submit Review".                                                                | -                                             | Review submitted successfully (pending moderation message appears).                                                                             |                                  |                           |                          |
| 3      | (On a different product or if allowed) Fill all required review fields. Select 5 star rating. | Rating: 5 stars                               | Review details entered, 5 stars selected.                                                                                                     |                                  |                           |                          |
| 4      | Click "Submit Review".                                                                | -                                             | Review submitted successfully (pending moderation message appears).                                                                             |                                  |                           |                          |
