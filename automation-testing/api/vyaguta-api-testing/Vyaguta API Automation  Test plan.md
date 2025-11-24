# Vyaguta API Automation Test plan

# 

Author : Kshitiz Rajan

# Table of Content

[**Introduction	3**](#introduction)

[Purpose	3](#purpose)

[Overview of the application	3](#overview-of-the-application)

[Audience	4](#audience)

[**Test Strategy / Approach	5**](#test-strategy-/-approach)

[**Test Scope	7**](#test-scope)

[**Test Objectives	8**](#test-objectives)

[**Test Environment	9**](#test-environment)

[**Test Schedule	10**](#test-schedule)

[**Test Resources	11**](#test-resources)

[**Entry/Exit Criteria	11**](#entry/exit-criteria)

[Entry Criteria	12](#entry-criteria)

[Exit Criteria	12](#exit-criteria)

[**Test Deliverables	13**](#test-deliverables)

[**References / Glossary	14**](#references-/-glossary)

# 

# Introduction {#introduction}

This test plan explains how we will do **automation testing** for the Vyaguta web application APIs using **Postman**. It tells what we will test, how we will test, and what resources we need.

The goal is to practice automated API testing, learn how to run tests automatically in Postman, and save time by testing many requests without doing them manually. We will also use **pre-request scripts** to set up data before sending a request, and **post-request scripts** to check if the API responses are correct.

# Purpose  {#purpose}

The purpose of this plan is to:

* Practice automation of API testing using Postman.  
* Test all **CRUD operations** (Create, Read, Update, Delete).  
* Check API responses with **valid and invalid data**.  
* Test authentication with **Bearer token**.  
* Use scripts to **prepare requests automatically** and **validate responses**.  
* Create reusable and easy-to-run automated tests.

The main goal is to learn automation in Postman and make testing faster and easier.

# Overview of the application {#overview-of-the-application}

Vyaguta is a web application with many APIs to manage events and users.In this practice, we will:

* Automate CRUD operations for events and other endpoints.  
* Check authentication using a token.  
* Use pre-request scripts to set data like date or user ID before sending requests.  
* Use test scripts to check the response automatically (status code, data, errors).  
* Use environment and collection variables to make tests reusable and easy to change.

This practice is for learning and gaining experience in automated API testing using Postman.

# Audience	 {#audience}

This test plan is for:

* **QA learners** who want to practice automation in Postman.  
* **Tutors or mentors** who guide and review the test results.

# Test Strategy / Approach {#test-strategy-/-approach}

We will do automation testing using **Postman** with pre**\-**request and test scripts.

1. **Authentication Testing**  
   * Use the Bearer token given by the tutor.  
   * Test with a valid token and also test requests without a token.

2. **CRUD Operations Testing**  
   * **Create (POST):** Add new events with valid and invalid data.  
   * **Read (GET):** Get event details using valid and invalid user IDs.  
   * **Update (PUT/PATCH):** Change event information and check if it updates correctly.  
   * **Delete (DELETE):** Remove events and confirm deletion.

3. **Pre-request Scripts**  
   * Run **before sending the request**.  
   * Set or change variables like `eventDate` or `userId`.

   * Example: pm.environment.set("eventDate", new Date().toISOString());

   

4. **Test Scripts (Post-request Scripts)**  
   * Run after sending the request.  
   * Check if the API response is correct.  
   * Example:

pm.test("Status code is 201", function () {

    pm.response.to.have.status(201);

});

pm.test("Event name is correct", function () {

    var jsonData \= pm.response.json();

    pm.expect(jsonData.name).to.eql(pm.environment.get("eventName"));

});

5. **Positive Testing**  
   * Test with valid data and check if the response is correct.

6. **Negative Testing**  
   * Test with invalid data or missing fields and check if the API returns the correct error.

7. **Environment and Collection Variables**  
   * Use variables like `baseUrl`, `userId`, `eventName`, `eventDescription` to make tests reusable.

8. **Documentation**  
   * Record test results: expected vs actual responses and any errors found.

This strategy helps us learn automation in Postman, cover all CRUD operations, test authentication, and use scripts to check responses automatically.

# Test Scope {#test-scope}

**In-Scope** (what we will test):

* **Authentication** – Test APIs with a valid token and without a token.  
* **CRUD Operations** – Test creating, reading, updating, and deleting events.  
* **Positive Testing** – Test APIs with correct data and check if responses are correct.  
* **Negative Testing** – Test APIs with wrong or missing data and check if proper error messages appear.  
* **Pre-request Scripts** – Set up dynamic data before sending requests (like event date or user ID).  
* **Test Scripts** – Automatically check responses after sending requests (status codes, fields, errors).  
* **Environment and Collection Variables** – Use variables like `baseUrl`, `userId`, `eventName`, etc., for easy and reusable testing.

**Out-of-Scope** (what we will not test):

* Frontend or UI testing of the Vyaguta website.  
* Load or performance testing of the APIs.  
* Integration with other systems outside the Vyaguta QA environment.  
* Manual testing (this plan focuses on automation using Postman).

## 

## 

## 

# Test Objectives {#test-objectives}

The objectives of this automation testing are:

* **Learn automation testing using Postman** – practice running automated API tests  
* **Verify CRUD operations** – ensure that creating, reading, updating, and deleting events works correctly.  
* **Check authentication** – test APIs with valid and missing tokens to make sure only authorized requests work.  
* **Validate responses automatically** – use test scripts to check status codes, response data, and error messages.  
  **Use dynamic data** – practice using environment and collection variables for reusable tests.  
* **Detect errors quickly** – identify problems in the APIs using automated tests instead of manual checking.  
* **Document results** – record automated test results and any issues found for review.

# Test Environment {#test-environment}

The testing of Sauce Demo will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| API environment | https://qa.vyaguta.lftechnology.com.np |
| Tools  | Postman desktop app |
| Environment Variables | Variables like `baseUrl`, `userId`, `eventName`, `eventDescription`, `eventLink`, `eventDate` for dynamic and reusable requests |
| Pre-request Scripts | Scripts that run before sending the request to set or update variables, generate timestamps, or prepare data |
| Post-request Scripts | Scripts that run after receiving the response to validate status codes, response body, fields, and error messages |
| Test Accounts | Provided by Sauce Demo: standard\_user, locked\_out\_user, problem\_user, performance\_glitch\_user, visibillity\_user  |
| Internet Connection | Stable internet connection required to send requests and get responses |
| Operating System  | Windows |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Prepare automation test plan, set up Postman environment and collection variables, get Bearer token | 1 day  |
| Test Case Design | Create automated test requests for all CRUD operations, authentication, and validations; add pre-request and test scripts | 1-2 days |
| Test Execution – Cycle 1 | Run automated tests with valid data, check responses, validate with test scripts, document results | 1-2 days |
| Test Execution – Cycle 2 | Run automated tests with invalid data, negative scenarios, and error handling; check responses with test scripts | 1 day |
| Bug Logging & Review | Record any issues found, review results with tutor or mentor | 1 day |
| Test Closure / Summary | Finalize automation test results, document learnings and observations | 1 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for Sauce Demo:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Test Data Resources | Valid and invalid payloads for CRUD operations Environment & collection variables (`userId`, `eventName`, `eventDescription`, `eventLink`, `eventDate`) |
| Skills / Knowledge | understanding of HTTP methods (GET, POST, PUT/PATCH, DELETE) Familiarity with Postman and API automation concepts Knowledge of authentication with Bearer token Understanding of pre-request and test scripts for automation |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* QA environment (`https://qa.vyaguta.lftechnology.com.np`) is ready.  
* Postman environment and collection variables are set up.  
* Bearer token is available for authentication.  
* Test data (valid and invalid) is prepared.  
* QA tester understands CRUD operations, Postman automation, and scripts.

  ### **Exit Criteria** {#exit-criteria}

* All planned automated tests are executed.  
* All critical or high-severity defects are logged.  
* No blocker issues remain.  
* Automated test results are documented and reviewed.  
* Learning objectives for automation practice are achieved.


# Test Deliverables {#test-deliverables}

* Automation test plan document.  
* Postman collection with all automated requests for CRUD operations and authentication.  
* Pre-request scripts to set up dynamic data before requests.  
* Test scripts to validate responses automatically.  
* Environment variables for dynamic and reusable testing (`baseUrl`, `userId`, `eventName`, `eventDescription`, etc.).  
* Test execution results and reports.  
* Logged defects or issues found during automated testing.  
* Summary of learnings and observations from the automation practice.


# References / Glossary  {#references-/-glossary}

**References:**

* Vyaguta QA environment: `https://qa.vyaguta.lftechnology.com.np`  
* Postman official documentation: [https://learning.postman.com](https://learning.postman.com)  
* Tutor-provided guidelines and API documentation.

**Glossary:**

* **API (Application Programming Interface):** A set of rules that allows one software application to talk to another.  
* **CRUD Operations:** Basic actions on data: Create, Read, Update, Delete.  
* **Bearer Token:** A type of authorization token used to access secure APIs.  
* **Environment Variable:** A value stored in Postman that can be reused in multiple requests.  
* **Pre-request Script:** Script that runs before sending a request to set or update variables.  
* **Test Script:** Script that runs after receiving a response to check if the API worked correctly.  
* **Positive Testing:** Testing with valid inputs to ensure the API works correctly.

* **Negative Testing:** Testing with invalid or missing inputs to ensure proper error handling.




# 

