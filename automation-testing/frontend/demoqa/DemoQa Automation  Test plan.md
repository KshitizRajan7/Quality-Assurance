# DemoQa Automation Test plan

# 

Author : Kshitiz Rajan

# Table of Content

[**Introduction	3**](#introduction)

[Purpose	3](#purpose)

[Overview of the application	3](#overview-of-the-application)

[Audience	4](#audience)

[**Test Strategy / Approach	5**](#test-strategy-/-approach)

[Functional Testing	5](#functional-testing)

[UI / Visual Testing	5](#ui-/-visual-testing)

[Negative Testing	5](#negative-testing)

[Reusability & Maintenance	5](#reusability-&-maintenance)

[Reporting	5](#reporting)

[**Test Scope	6**](#test-scope)

[**Test Objectives	7**](#test-objectives)

[**Test Environment	8**](#test-environment)

[**Test Schedule	9**](#test-schedule)

[**Test Resources	10**](#test-resources)

[**Entry/Exit Criteria	10**](#entry/exit-criteria)

[Entry Criteria	11](#entry-criteria)

[Exit Criteria	11](#exit-criteria)

[**Test Deliverables	12**](#test-deliverables)

[**References / Glossary	13**](#references-/-glossary)

[References	13](#references)

[Glossary	13](#glossary)

# 

# Introduction {#introduction}

This test plan is for **automating the Forms page** of DemoQA. On this page, users can enter information, select options, click buttons, and submit the form.

Automation testing will check that all fields, buttons, checkboxes, radio buttons, and dropdowns work correctly and give consistent results every time.

# Purpose  {#purpose}

The purpose of this test plan is to make sure the **Forms page** works correctly using automation.

It will help to:

* Automatically check input fields, checkboxes, radio buttons, dropdowns, and buttons

* Confirm the form can be submitted successfully

* Find any problems or bugs automatically

* Save time by avoiding repetitive manual testing

# Overview of the application {#overview-of-the-application}

The DemoQA Forms page has text fields, radio buttons, checkboxes, dropdowns, and a submit button.

This plan will automate tests to check:

* All fields work correctly

* Validation messages appear for wrong input

* Form submits correctly

* The page elements behave as expected

# Audience	 {#audience}

This test plan is for the QA tester (you) who will write and run automation scripts for the DemoQA Forms page.

It can also help developers or other team members understand what is being tested and how automation is done.

# Test Strategy / Approach {#test-strategy-/-approach}

The testing of DemoQA Forms will be done using **automation scripts** with **Cypress** to verify frontend functionality efficiently.

### **Functional Testing** {#functional-testing}

* Automate tests for input fields, radio buttons, checkboxes, and dropdowns  
* Verify submit button functionality and form submission  
* Check validation messages for invalid or missing input

### **UI / Visual Testing** {#ui-/-visual-testing}

* Automate verification of labels, buttons, messages, and layout  
* Check colors, fonts, alignment, and hover/click/focus effects

### **Negative Testing** {#negative-testing}

* Test invalid or empty input automatically  
* Verify proper error messages appear for incorrect data

### **Reusability & Maintenance** {#reusability-&-maintenance}

* Use reusable scripts for common actions like input and submit  
* Store test data in JSON or fixture files for multiple scenarios

### **Reporting** {#reporting}

* generate automated reports showing passed/failed tests  
* Capture screenshots for failed tests

# Test Scope {#test-scope}

The automation testing will cover the main features of the DemoQA Forms page:

* Input fields for name, email, and other personal information

* Radio buttons and checkboxes

* Dropdown menus

* Submit button functionality

* Validation messages for incorrect or missing input

* Visibility and functionality of all page elements

**Out of Scope:**

* Browser compatibility testing beyond default supported browsers

* Performance testing

* Security testing

This scope ensures that the important functions of the Forms page are tested automatically while keeping the work manageable.

## 

## 

## 

# Test Objectives {#test-objectives}

The objectives of automation testing for the DemoQA Forms page are:

* To check that all input fields accept valid data and show correct messages for invalid data

* To ensure radio buttons, checkboxes, and dropdown menus work correctly

* To confirm the submit button functions properly and the form can be submitted

* To verify that validation messages, modal and page elements display correctly

* To automatically detect any defects or issues during testing

These objectives guide the automation effort and ensure the critical parts of the Forms page are tested reliably.

# Test Environment {#test-environment}

The testing of DemoQa will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| Web Browser | Google Chrome, Edge |
| Internet Connection | Stable connection required |
| Device | Desktop , Laptop |
| Automation Tools  | Cypress (installed via Node.js) , VS Code |
| Dependencies | Cypress Drivers,Node.js, required Npm packages  |
| Operating System  | Windows |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Writing the automation test plan | 0.5 day  |
| Test Case Design | Installing Cypress, setting up test accounts and dependencies | 0.5 day |
| Automation Script Design | Creating scripts for input fields, buttons, checkboxes, radio buttons, and dropdowns | 1 day |
| Test Execution – Input Fields | Running automated tests for text fields | 0.5 day |
| Test Execution – Options | Running automated tests for radio buttons, checkboxes, and dropdowns | 0.5 day |
| Test Execution – Submit Button | Running automated tests for form submission and validation messages  | 0.5 day |
| Test Reporting | Reviewing automated test results, logging any issues, and generating reports | 0.5 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for DemoQa:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Automation Tool | Cypress |
| Test Data | Fixtures or Json files used in automation scripts |
| Documentation Tools | Test plan, test cases, bug reporting sheet |
| Reporting Tool | Cypress built-in reporter or any external reporter for logs and results |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* Automation test plan and test cases are prepared

* Test environment is set up with Cypress, browsers, and IDE

* Test data (fixtures or JSON files) is ready

  ### **Exit Criteria** {#exit-criteria}

* All planned automated test cases have been executed

* All critical and major defects found during automation are logged

* Test execution reports, screenshots, and logs are generated

* Automation scripts are reviewed and updated if needed  
  


# Test Deliverables {#test-deliverables}

The following items will be produced and used during the automation testing of the DemoQA Forms page:

* **Automation Test Plan Document** – outlines the approach, scope, and objectives

* **Automation Test Scripts** – Cypress scripts for input fields, buttons, checkboxes, radio buttons, dropdowns, and form submission

* **Test Data Files** – JSON or fixture files used in automated tests

* **Cypress Configuration Files** – project setup and environment configuration

* **Test Execution Report** – report showing passed and failed automated tests

* **Screenshots / Videos** – captured by Cypress during test runs, especially for failures

* **Defect Report** – issues found during automation

* **Final Automation Summary Report** – overview of automation coverage and results

These deliverables document the automation testing process and provide evidence of results.

# References / Glossary  {#references-/-glossary}

### **References** {#references}

* DemoQA website: [https://demoqa.com](https://demoqa.com)

* DemoQA Forms page documentation

* Cypress official documentation

* QA best practices and guidelines

* Project requirements or specifications

  ### **Glossary** {#glossary}

* **Automation Testing:** Using scripts to test application functionality instead of manual steps

* **Cypress:** A JavaScript-based tool for automating web application testing

* **Test Script:** Code written to automate a test case

* **Fixture:** Test data file used in automation scripts

* **Assertion:** A check to verify that the actual result matches the expected result

* **Test Runner:** Tool that executes automation scripts (Cypress Test Runner)

* **Report:** Output showing which tests passed, failed, or were blocked

* **CI/CD:** Continuous Integration / Continuous Delivery pipeline used to run automated tests automatically

* **Selector:** Method to locate elements on a web page (e.g., CSS selector)  
  




# 

