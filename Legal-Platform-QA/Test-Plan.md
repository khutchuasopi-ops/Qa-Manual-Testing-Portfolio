# Test Plan — Legal Platform QA

## 1. Objective

The goal of testing was to check whether the main features of the legal platform work as expected.

The testing focused on common user actions, input validation, data consistency, search, file handling, and AI-assisted features.

---

## 2. Scope

The following areas were included in testing:

* Dashboard
* Repository
* Documents
* File Upload
* File Replacement
* Templates
* Events
* Workflows
* AI Assistant
* Search
* Recycle Bin
* Playbook Generation

---

## 3. Testing Types

The following manual testing types were used:

* Functional Testing
* Negative Testing
* Boundary Value Testing
* Input Validation
* Exploratory Testing
* Regression Testing
* UI Testing
* Data Consistency Testing
* Search and Filtering Testing
* Error Handling

---

## 4. Functional Testing

Functional testing was used to check the main features and user flows.

Examples included:

* creating documents
* uploading files
* replacing files
* creating templates
* creating events
* searching for information
* deleting and restoring items
* using workflows
* interacting with the AI Assistant

---

## 5. Negative Testing

Negative testing was used to check how the application behaves with invalid or unexpected input.

Examples:

* empty required fields
* invalid names
* invalid values
* incorrect input formats
* unsupported actions

The expected result was that the application should prevent invalid actions and show an appropriate message where required.

---

## 6. Boundary Testing

Boundary values were tested where fields had specific limits.

The testing included values such as:

* minimum allowed length
* maximum allowed length
* values below the limit
* values above the limit
* empty values

---

## 7. Data Consistency

Data consistency was checked after actions that could change or replace information.

Examples:

* replacing a file
* deleting an item
* restoring an item
* updating information
* refreshing the page after changes

The main goal was to check that the displayed data remained correct after these actions.

---

## 8. Search Testing

Search functionality was tested using different types of input.

The testing included:

* valid search terms
* partial search terms
* empty search
* invalid search
* filtering
* checking search results

The results were checked to make sure they matched the search criteria.

---

## 9. File Testing

File-related functionality was tested around:

* file upload
* file replacement
* file visibility
* deleted files
* restored files
* data after replacement

Special attention was given to whether the correct file and information were displayed after an update.

---

## 10. AI Assistant Testing

The AI Assistant was tested manually using different inputs and requests.

The testing focused on:

* basic interaction
* different user inputs
* generated responses
* handling unexpected input
* general usability

The testing was focused on the visible behavior of the feature rather than the internal AI model.

---

## 11. Test Environment

* **Environment:** Staging
* **Testing:** Manual
* **Browser:** Chrome
* **Documentation:** Markdown
* **Defect Tracking:** GitHub

Exact browser version and test dates are not included where they were not recorded during testing.

---

## 12. Test Data

Test data was created or entered manually during testing.

Examples included:

* document names
* template names
* event names
* search terms
* valid and invalid field values
* uploaded files
* boundary values

No real confidential or personal data is included in the portfolio.

---

## 13. Entry Criteria

Testing could start when:

* the staging environment was available
* the main features were accessible
* required test data was available
* the application was stable enough for manual testing

---

## 14. Exit Criteria

Testing was considered complete when:

* planned test cases were executed
* exploratory testing was performed
* identified bugs were documented
* important failed scenarios were reviewed
* test results were recorded
* regression testing was performed where applicable

---

## 15. Bug Reporting

Bugs were documented with the following information:

* Bug ID
* Title
* Environment
* Steps to Reproduce
* Actual Result
* Expected Result
* Severity
* Priority
* Status

Each bug was reported separately in the `Bug-Reports` folder.

---

## 16. Known Testing Limitations

The testing was performed as manual black-box testing.

The following areas were not included:

* source code testing
* automated testing
* API testing
* database testing
* performance testing
* load testing
* security penetration testing

The internal implementation of the AI features was also outside the testing scope.

---

## 17. QA Deliverables

The project includes:

* Test Plan
* Test Scenarios
* Test Cases
* Checklists
* Exploratory Testing
* Test Execution
* Bug Reports
* Case Study

---

## 18. Test Plan Summary

The main focus of this test plan was to cover the core user flows of the platform and identify problems that could affect normal usage.

Special attention was given to:

* input validation
* file handling
* data consistency
* search
* boundary values
* AI-assisted functionality
* user interface behavior
* negative scenarios

Testing results and identified bugs are documented in the related project files.
