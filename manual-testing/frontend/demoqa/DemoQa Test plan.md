# DemoQa Manual Test plan

# 

Author : Kshitiz Rajan

# Table of Content

[**Introduction	3**](#introduction)

[Purpose	3](#purpose)

[Overview of the application	3](#overview-of-the-application)

[Audience	3](#audience)

[**Test Strategy / Approach	4**](#test-strategy-/-approach)

[Functional Testing	4](#functional-testing)

[UI / Visual Testing	4](#ui-/-visual-testing)

[Negative Testing	4](#negative-testing)

[Usability Testing	4](#usability-testing)

[Reporting	4](#reporting)

[**Test Scope	5**](#test-scope)

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

This test plan is for the **Forms** page of DemoQA. On this page, users can enter personal information, select options, click buttons, and submit the form.

We will check if all the fields, buttons, checkboxes, radio buttons, and dropdowns work correctly and show proper messages when needed.

## Purpose  {#purpose}

The purpose of this test plan is to make sure the **Forms** page works properly.

We want to:

* Check that all fields accept correct data and show errors for wrong data

* Make sure buttons, checkboxes, radio buttons, and dropdowns work

* Check that the form can be submitted successfully

* Find any problems or bugs

## Overview of the application {#overview-of-the-application}

The DemoQA Forms module includes text fields, radio buttons, checkboxes, dropdowns, and submit buttons.

This test plan covers the verification of field behavior, input validations, data submission, and the overall functionality of the Forms page.

## Audience	 {#audience}

This test plan is prepared for the QA tester who will perform all the testing activities for Sauce Demo.

It is mainly for personal guidance to ensure testing is organized, complete, and easy to track.

# Test Strategy / Approach {#test-strategy-/-approach}

The testing of DemoQA Forms will be done manually to verify frontend functionality.

### **Functional Testing** {#functional-testing}

* Check all input fields accept valid data  
* Verify radio buttons, checkboxes, and dropdowns work correctly  
* Test the submit button for successful form submission  
* Validate error messages for invalid or missing input

### **UI / Visual Testing** {#ui-/-visual-testing}

* Ensure all labels, buttons, and messages are visible and aligned correctly  
* Check colors, fonts, and layout  
* Verify hover, click, and focus effects

### **Negative Testing** {#negative-testing}

* Enter invalid or empty data in required fields  
* Test incorrect email or phone number formats  
* Verify appropriate error messages are displayed

### **Usability Testing** {#usability-testing}

* Ensure the form is easy to use and intuitive  
* Verify users can fill and submit the form without confusion

### **Reporting** {#reporting}

* Record test results in a spreadsheet or document  
* Capture screenshots for any defects  
* Prepare a Test Execution Summary showing passed/failed cases

# Test Scope {#test-scope}

The testing will cover the main functionalities of the DemoQA Forms page, including:

* Input fields for personal and contact information

* Radio buttons and checkboxes

* Dropdown menus

* Submit button functionality

* Validation messages for incorrect or missing input

* User interface elements such as labels, buttons, and messages

**Out of Scope:**

* Browser compatibility testing

* Performance testing

* Security testing

This scope ensures that the key functionalities of the Forms page are tested thoroughly while keeping the testing process manageable.

## 

## 

## 

# Test Objectives {#test-objectives}

The objectives of testing the DemoQA Forms page are:

* To verify that all input fields accept valid data and provide correct validation for invalid input

* To ensure that radio buttons, checkboxes, and dropdown menus function correctly

* To confirm that the submit button works and the form can be submitted successfully

* To validate that all messages, labels, and UI elements are displayed correctly

* To identify and report any defects or issues found during testing

These objectives guide the testing process and ensure that all critical aspects of the Forms page are properly validated.

# Test Environment {#test-environment}

The testing of Sauce Demo will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| Web Browser | Google Chrome, Edge |
| Internet Connection | Stable connection required |
| Device | Desktop , Laptop |
| Operating System | Windows |
| Tools | Browser for manual testing, google sheets for logging test cases and defects |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Writing the test plan document | 0.5 day  |
| Test Case Design | Creating test cases for all input fields, buttons and validations | 1 day |
| Test Environment Setup | Preparing browser and devices | 0.5 day |
| Test Execution – Input Fields | Testing all text fields for valid and invalid inputs | 0.5 day |
| Test Execution – options | Testing radiobuttons, checkboxes and dropdowns | 0.5 day |
| Test Execution –  Submit Functionality | Testing the form submission and validation message (Modal) | 0.5 day |
| Test Reporting | Logging defects, preparing test execution summary | 0.5 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for Sauce Demo:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Documentation Tools | Test plan, test cases, bug reporting sheet |
| Reporting Tool | Google Sheets, or any simple tracker |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* Test plan and test cases are prepared

* Test environment is ready, including browser and device setup

* Required test data is available  
  

### **Exit Criteria** {#exit-criteria}

* All planned test cases have been executed

* All critical and major defects are logged

* Test results and execution summary are documented

* Any issues found during testing are communicated for resolution


# Test Deliverables {#test-deliverables}

The following items will be produced and used during the testing of the DemoQA Forms page:

* **Test Plan Document** – outlines the testing approach, scope, and objectives

* **Test Cases Document** – detailed steps for testing all form fields, options, and validations

* **Bug/Defect Report** – records of any issues found during testing

* **Test Execution Report or Summary** – overview of test results, including passed and failed test cases

* **Screenshots or Evidence of Testing Results** – visual proof of test execution and any defects

These deliverables provide documentation and evidence of the testing process and results.

# References / Glossary  {#references-/-glossary}

### **References** {#references}

* DemoQA website: [https://demoqa.com](https://demoqa.com)

* DemoQA Forms page documentation

* QA best practices and guidelines

* Project requirements or specifications

  ### **Glossary** {#glossary}

* **QA (Quality Assurance):** The process of ensuring that the software meets expected standards and works correctly

* **Test Case:** A set of steps to verify a specific functionality of the application

* **Defect / Bug:** Any issue or error found in the application

* **Test Plan:** A document that outlines the testing scope, objectives, approach, and resources

* **Validation:** Checking if input data meets the expected rules or criteria

* **Execution Report:** A summary of test results including passed, failed, and blocked cases

* **Test Environment:** The setup used for testing, including browser, device, and accounts




# 

