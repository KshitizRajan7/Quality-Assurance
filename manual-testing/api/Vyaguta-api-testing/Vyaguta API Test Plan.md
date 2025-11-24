# Vyaguta API Test plan

# 

Author : Kshitiz Rajan

# Table of Content

[**Introduction	3**](#introduction)

[Purpose	3](#purpose)

[Overview of the application	3](#overview-of-the-application)

[Audience	3](#audience)

[**Test Strategy / Approach	4**](#test-strategy-/-approach)

[Approach	4](#approach)

[**Test Scope	5**](#test-scope)

[In-Scope	5](#in-scope)

[Out-of-Scope	5](#out-of-scope)

[**Test Objectives	6**](#test-objectives)

[**Test Environment	7**](#test-environment)

[**Test Schedule	8**](#test-schedule)

[**Test Resources	9**](#test-resources)

[**Entry/Exit Criteria	9**](#entry/exit-criteria)

[Entry Criteria	10](#entry-criteria)

[Exit Criteria	10](#exit-criteria)

[**Test Deliverables	11**](#test-deliverables)

[**References / Glossary	12**](#references-/-glossary)

[References	12](#references)

[Glossary	12](#glossary)

# 

# Introduction {#introduction}

This test plan outlines the approach for **practicing manual API testing** on the Vyaguta web application, provided by Leapfrog. It covers testing of API endpoints using Postman, focusing on sending requests with valid and invalid data, verifying authentication with tokens, and observing API responses. The plan is intended to help learners gain hands-on experience in API testing, understand response validation, and document results effectively.

## Purpose  {#purpose}

The purpose of this test plan is to practice manual API testing of Vyaguta API endpoints. It focuses on understanding how to send API requests, use tokens for authentication, validate responses, and handle positive and negative scenarios. The goal is to gain hands-on experience in testing APIs, working with environment and collection variables, and documenting results effectively.

## Overview of the application {#overview-of-the-application}

Vyaguta is a web application with multiple API endpoints for managing events and user data. This manual API testing exercise focuses on learning how to test these APIs using **Postman**. The testing includes sending requests with valid and invalid payloads, verifying responses, checking authentication with Bearer tokens, and practicing CRUD operations (Create, Read). Environment and collection variables are used to make testing dynamic and reusable. The purpose is purely educational, to gain practical experience in API testing concepts and workflows.

## Audience	 {#audience}

This test plan is intended for:

* **QA Learners / Trainees** – practicing manual API testing using Postman.

* **Tutors / Mentors** – providing guidance, reviewing test results, and validating the testing approach.

# Test Strategy / Approach {#test-strategy-/-approach}

The testing will be performed manually using Postman, focusing on understanding API behavior, response validation, and authentication mechanisms.

### **Approach** {#approach}

1. **Authentication Testing**  
   * Use the **Bearer token** provided by the tutor.  
   * Test API requests with valid and missing tokens to verify authorization.

2. **CRUD Operations Testing**  
   * **Create (POST)**: Add new events with valid and invalid payloads.  
   * **Read (GET)**: Fetch events using valid and invalid `userId`.  
   * **Update (PUT / PATCH)**: Modify event data and verify updates.  
   * **Delete (DELETE)**: Remove events and validate deletion.

3. **Positive Testing**  
   * Send valid requests across all CRUD operations.  
   * Verify correct status codes (`200 OK`, `201 Created`, `204 No Content`) and response data.

4. **Negative Testing**  
   * Send invalid requests (wrong fields, missing required data, invalid user ID, unauthorized access).  
   * Validate proper error codes (`400 Bad Request`, `401 Unauthorized`, `404 Not Found`) and error messages.

5. **Additional Validations**  
   * Input validation (required fields, data types, formats).  
   * Response structure and field consistency.  
   * Edge cases and boundary values where applicable.

6. **Use of Environment & Collection Variables**  
   * Dynamic data such as `baseUrl`, `userId`, `eventName`, `eventDescription`, etc., will be stored as variables.  
   * Reuse variables across requests for consistent testing.

7. **Documentation**

   * Record all request inputs, expected vs actual results, and status codes.  
   * Log any defects or discrepancies for review.

# Test Scope {#test-scope}

### **In-Scope** {#in-scope}

The following areas will be tested manually using Postman:

* **Authentication / Authorization**  
  * Requests with valid token  
  * Requests without token  
  * Requests with invalid token (if applicable)

* **CRUD Operations**  
  * **Create (POST)**: Add new events with valid and invalid payloads  
  * **Read (GET)**: Fetch events by valid and invalid `userId`  
  * **Update (PUT / PATCH)**: Modify existing event data  
  * **Delete (DELETE)**: Remove events and validate deletion

* **Positive & Negative Testing**  
  * Validate API responses with correct and incorrect data  
  * Test required field validations, input formats, and error messages

* **Environment & Collection Variables**  
  * Use dynamic variables like `baseUrl`, `userId`, `eventName`, `eventDescription`, etc., to make requests reusable

* **Response Verification**  
  * Status codes (200, 201, 204, 400, 401, 404\)  
  * Response body structure  
  * Error handling messages

### **Out-of-Scope** {#out-of-scope}

* Full production-level load/performance testing  
* UI or frontend testing  
* Complex integration with other systems (if not provided in practice environment)  
* Automated testing (covered in separate plan, if any)

## 

# Test Objectives {#test-objectives}

The objectives of this manual API testing exercise are:

1. **Learn API Testing Fundamentals**  
   * Gain hands-on experience with sending API requests and understanding responses.

2. **Verify Authentication and Authorization**  
   * Test requests with valid, missing, or invalid tokens using Bearer token authentication.

3. **Validate CRUD Operations**  
   * Ensure Create, Read, Update, and Delete APIs work correctly with valid and invalid data.

4. **Check Data Validation and Error Handling**  
   * Verify proper handling of missing fields, incorrect data types, invalid user IDs, and other negative scenarios.

5. **Practice Using Environment and Collection Variables**  
   * Use variables like `baseUrl`, `userId`, `eventName`, etc., to make requests dynamic and reusable.

6. **Document Testing Results**  
   * Record request inputs, expected and actual responses, and log any defects found during testing.

**Overall Goal:** To gain practical experience and understanding of manual API testing workflows, validations, and best practices in a controlled learning environment.

# Test Environment {#test-environment}

The testing of Sauce Demo will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| Tools  | Postman , Google sheets / docs |
| API environment | https://qa.vyaguta.lftechnology.com.np |
| Authentication | Bearer Token |
| Environment Variables | baseUrl, eventName, eventDescription, eventLink, eventDate, userId |
| Supported System | Postman desktop apps(Windows/ maxOS) / web version |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Prepare test plan, set up Postman environment and collection variables | 1 day  |
| Test Case Design | Create manual test cases for all CRUD operations, authentication, and validations | 1-2 days |
| Test Execution \- Cycle1 | Execute test cases with valid data, verify responses, document results | 1-2 days |
| Test Execution – Cycle2 | Execute test cases with invalid data, negative scenarios, and error handling | 1 day |
| Bug Logging & Review | Record any discrepancies, review results with tutor | 1 day |
| Test Closure / Summary | Finalize test results, document learnings and observations | 0.5 \-1 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for Sauce Demo:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Test Data Resources | Valid and invalid payloads for CRUD operations Environment & collection variables (`userId`, `eventName`, `eventDescription`, etc.) |
| Skills / Knowledge | Understanding of HTTP methods (GET, POST, PUT/PATCH, DELETE) Familiarity with Postman and API testing concepts Knowledge of authentication with Bearer token |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* TQA environment (`qa.vyaguta.lftechnology.com.np`) is accessible  
* Postman environment and collection variables are set up  
* Token provided by tutor is available  
* Test data (valid & invalid payloads) prepared  
* QA tester understands CRUD operations and API testing workflow

### **Exit Criteria** {#exit-criteria}

* All planned test scenarios executed (positive & negative)  
* All critical and high-severity defects logged  
* No blocker issues remain unresolved  
* Test results documented and reviewed  
* Learning objectives for API testing practice achieved

# Test Deliverables {#test-deliverables}

The following items will be produced and used during the testing of Sauce Demo:

* **Test Plan** – Outlines the testing approach, scope, objectives, environment, resources, and schedule.

* **Manual Test Cases** – Covers all CRUD operations, authentication, positive and negative scenarios.

* **Postman Collection** – Contains API requests with environment and collection variables for easy execution and reuse.

* **Test Data** – Sample payloads (valid and invalid) used for testing each endpoint.

* **Defect / Bug Log** – Records any issues found during testing, including steps to reproduce, status, and severity.

* **Test Summary / Report** – Summarizes test execution, results, defects discovered, and key learnings from the practice exercise.


# References / Glossary  {#references-/-glossary}

### **References** {#references}

* Vyaguta QA Environment: `https://qa.vyaguta.lftechnology.com.np`

* Postman Documentation: [https://learning.postman.com/docs/getting-started/introduction/](https://learning.postman.com/docs/getting-started/introduction/)

* HTTP Status Codes: [https://developer.mozilla.org/en-US/docs/Web/HTTP/Status](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)

* Leapfrog QA Tutor Guidelines / Instructions

  ### **Glossary** {#glossary}

* **API (Application Programming Interface)** – A set of rules that allows applications to communicate with each other.

* **CRUD** – Create, Read, Update, Delete; the four basic operations for managing data.

* **Bearer Token** – A security token used in authentication to access protected API endpoints.

* **Environment Variables** – Variables in Postman used to store values like `baseUrl` or `userId` for dynamic testing.

* **Collection Variables** – Variables stored at the collection level in Postman, e.g., `token`.

* **Positive Testing** – Testing with valid data to verify expected behavior.

* **Negative Testing** – Testing with invalid or unexpected data to verify proper error handling.

* **QA (Quality Assurance)** – The practice of ensuring a product meets specified requirements and quality standards.




# 

