# 🧪 Manual Test Suite: Luma E-commerce Platform (Magento Demo)

This repository showcases a manual test suite designed for the Luma e-commerce platform, the Magento demo store available at [https://magento.softwaretestingboard.com/](https://magento.softwaretestingboard.com/).

## 🚀 Project Overview

This project demonstrates a comprehensive manual Quality Assurance approach to testing a typical e-commerce application. It includes a lightweight test plan, detailed test cases covering core functionalities, and sample bug reports to illustrate defect documentation.

The primary goals are to:
* Demonstrate a structured approach to manual testing.
* Showcase the creation of clear, effective, and well-organized test cases.
* Illustrate understanding of various test design techniques and testing types.
* Provide a foundational set of manual tests that could inform future automation efforts.

**Application Under Test (AUT):** [https://magento.softwaretestingboard.com/](https://magento.softwaretestingboard.com/)

---

## 🛍️ Modules Covered

The test suite focuses on the core e-commerce functionalities:
* 👤 **User Account Management:** Registration, Login, Logout, (Conceptual: Password Recovery).
* 🔍 **Product Browse & Search:** Category Navigation, Keyword Search, Filtering, Sorting.
* 📄 **Product Details Page (PDP):** Viewing Details, Selecting Options (size, color), Quantity Adjustment, Adding to Cart.
* 🛒 **Shopping Cart Management:** Viewing Cart, Updating Quantities, Removing Items.
* 💳 **Checkout Process:** For both registered and guest users, including shipping and (mock) payment steps.

---

## 🛠️ Testing Techniques & Approach

* **Functional Testing:** Verifying features against expected e-commerce behaviors.
* **Positive Testing:** Ensuring the application works with valid inputs and user flows.
* **Negative Testing:** Challenging the system with invalid inputs and error conditions.
* **Boundary Value Analysis (BVA):** Testing at the edges of input ranges (e.g., quantity fields).
* **Equivalence Partitioning (EP):** Grouping inputs into classes to reduce test case redundancy.
* **Exploratory Testing (Conceptual):** While test cases are documented, an exploratory mindset was used to identify scenarios.
* **UI/UX Testing:** Assessing visual presentation and ease of use.
* **Basic Input Validation:** Checking how the system handles simple invalid data entries.

---

## 📁 Key Artifacts & Deliverables

This repository contains the following key deliverables:

1.  **📄 Test Plan Document**
    * **Location:** [./Test_Plan.md](./Test_Plan.md)
    * **Description:** Outlines the scope, objectives, test strategy, and resources for this testing effort.

2.  **🧪 Detailed Test Cases**
    * **Location:** [./Test_Cases/](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases) (Organized into sub-folders by module)
    * **Description:** Meticulously crafted test cases in Markdown (`.md`) format. Each file represents an individual test case detailing steps, preconditions, and expected results. They are categorized by module for clarity and ease of navigation.
        * [User Account Management](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases/User_Account_Management)
        * [Product Browse & Search](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases/Product%20Browse%20%26%20Search)
        * [Product Detail Page](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases/Product%20Detail%20Page)
        * [Shopping Cart](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases/Shopping%20Cart)
        * [Checkout Process](https://github.com/QualitasPrima/manual-test-magento-suite/tree/main/Test_Cases/Checkout%20Process)

3.  **🐞 Sample Bug Report**
    * **Location:** [./Bug_Report_Sample.md](./Bug_Report_Sample.md)
    * **Description:** An example of a detailed bug report, demonstrating clear communication of a defect, including steps to reproduce, expected vs. actual results, severity, and priority.

---

## 📈 Skills Demonstrated

This project highlights abilities in:
* Manual Testing Fundamentals & Best Practices
* Test Planning & Strategy Development
* Comprehensive Test Case Design (Positive, Negative, Edge, Boundary)
* Requirement Analysis (Implicit, based on standard e-commerce functionality)
* Effective Bug Reporting & Documentation
* Attention to Detail & Thoroughness
* Understanding of E-commerce Workflows
* Project Organization & Documentation (using Markdown and GitHub)

---

## 🎯 Next Steps (Potential Enhancements)

This manual testing suite lays a strong foundation. Future enhancements could include:
* 🤖 **Automated Test Suite:** Developing automated End-to-End (E2E) tests for key user flows using frameworks like Cypress or Playwright (linking to a future repository).
* 🔗 **API Testing:** Implementing API tests for backend validation of the e-commerce platform (linking to a future repository).
* 🔄 **CI/CD Integration:** Incorporating automated tests into a continuous integration pipeline using GitHub Actions.
* ♿ **Accessibility Testing:** Performing basic accessibility checks (e.g., WCAG AA).
* 📱 **Mobile Responsiveness Testing:** More detailed checks across various device emulations.

---

## 👤 Author

**David Jenkins (QualitasPrima)**
Senior QA Engineer | Manual & Automation Testing | Agile | Cypress / Playwright
[LinkedIn](https://www.linkedin.com/in/davidjenkins-qa/)*
