# Test Case: TC_PDP_REVIEW_002 - Reviews - Submit a Valid Review When Logged In

* **Module:** Product Detail Page
* **Feature:** Product Reviews
* **Objective:** Verify that a logged-in user can successfully submit a valid product review.
* **Priority:** High

**Preconditions:**
1.  User is logged into their account.
2.  User is on the PDP of any product.
3.  User has not reviewed this specific product before with this account (or system allows multiple reviews, which is less common).

---
**Test Execution:**

| Step # | Test Step Description                                                                 | Test Data (if applicable)                     | Expected Result                                                                                                                               | Actual Result (during execution) | Status (during execution) | Notes (during execution) |
|--------|---------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|---------------------------|--------------------------|
| 1      | Navigate to the "Reviews" tab on the PDP.                                             | -                                             | Review submission form is visible. Nickname field might be pre-filled with user's name.                                                         |                                  |                           |                          |
| 2      | Select a star rating (e.g., 5 stars).                                                 | Rating: 5 stars                               | Rating is selected.                                                                                                                           |                                  |                           |                          |
| 3      | Enter a valid Nickname (if not pre-filled or to change).                              | Nickname: `HappyShopper`                      | Nickname is entered.                                                                                                                          |                                  |                           |                          |
| 4      | Enter a valid Summary for the review.                                                 | Summary: `Great Product!`                       | Summary is entered.                                                                                                                           |                                  |                           |                          |
| 5      | Enter valid text in the "Review" textarea.                                            | Review: `I am very satisfied with this purchase.` | Review text is entered.                                                                                                                       |                                  |                           |                          |
| 6      | Click the "Submit Review" button.                                                     | -                                             | 1. A success message is displayed (e.g., "You submitted your review for moderation."). <br> 2. The review may not appear immediately if moderation is pending. |                                  |                           |                          |
