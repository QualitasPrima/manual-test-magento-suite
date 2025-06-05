# Test Case: TC_PDP_REVIEW_003 - Reviews - Attempt to Submit Review with Missing Required Fields

* **Module:** Product Detail Page
* **Feature:** Product Reviews
* **Objective:** Verify that the system prevents review submission if required fields (e.g., rating, summary, review text) are missing and displays appropriate error messages.
* **Priority:** High

**Preconditions:**
1.  User is logged in and on the PDP "Reviews" tab, viewing the review submission form.

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Do not select a star rating. Fill in Nickname, Summary, and Review text.              | -                                             | Star rating remains unselected.                                                                                                               |                                  |                           |                          |
| 2      | Click "Submit Review".                                                                | -                                             | 1. Review is not submitted. <br> 2. An error message is displayed for the missing Rating (e.g., "Please select a rating.").                     |                                  |                           |                          |
| 3      | Select a star rating. Clear the "Summary" field. Fill other fields.                   | Summary: (empty)                              | Summary field is empty.                                                                                                                       |                                  |                           |                          |
| 4      | Click "Submit Review".                                                                | -                                             | 1. Review is not submitted. <br> 2. An error message is displayed for the missing Summary (e.g., "This is a required field.").                 |                                  |                           |                          |
| 5      | (Similarly test for other required fields like Review text and Nickname if applicable) | -                                             | Appropriate error messages appear for each missing required field.                                                                              |                                  |                           |                          |
