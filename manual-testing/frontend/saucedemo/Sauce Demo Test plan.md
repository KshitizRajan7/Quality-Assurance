# Sauce Demo Manual Test plan

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

[Usability Testing	5](#usability-testing)

[Cross-browser Testing	5](#cross-browser-testing)

[Reporting	5](#reporting)

[**Test Scope	6**](#test-scope)

[In-scope features	6](#in-scope-features)

[**Test Objectives	7**](#test-objectives)

[**Test Environment	8**](#test-environment)

[**Test Schedule	9**](#test-schedule)

[**Test Resources	10**](#test-resources)

[**Entry/Exit Criteria	10**](#entry/exit-criteria)

[Entry Criteria	11](#entry-criteria)

[Exit Criteria	11](#exit-criteria)

[**Test Deliverables	12**](#test-deliverables)

[**References / Glossary	13**](#references-/-glossary)

# 

# Introduction {#introduction}

This test plan is prepared for **Sauce Demo**, a sample e-commerce website provided by Sauce Labs. The website is used to practice testing and automation skills.  
The test plan will guide the QA team on what to test, how to test, and what tools to use, ensuring that the testing process is organized and effective.

## Purpose  {#purpose}

The purpose of this test plan is to ensure that Sauce Demo works correctly and provides a smooth experience for users.

It helps the QA team to:

* Identify bugs or issues in the website

* Verify that all features like login, product sorting, cart, and checkout are working as expected

* Make sure the website behaves consistently and reliably

This test plan acts as a guide for testing activities so that testing is organized, complete, and efficient.

## Overview of the application {#overview-of-the-application}

Sauce Demo is a sample e-commerce website designed for practicing testing skills. Users can log in, view products, sort them by name or price, add items to the cart, and complete the checkout process.

The website also includes different types of user accounts to test various scenarios, such as a standard user, a locked-out user, a problem user, and a performance glitch user.

This test plan will cover testing of all main features and workflows to make sure the website works as expected and is easy to use.

## Audience	 {#audience}

This test plan is prepared for the QA tester who will perform all the testing activities for Sauce Demo.

It is mainly for personal guidance to ensure testing is organized, complete, and easy to track.

# Test Strategy / Approach {#test-strategy-/-approach}

The testing of Sauce Demo will be done using a manual approach for now.

### **Functional Testing** {#functional-testing}

* Test login/logout with valid and invalid credentials  
* Verify product listing, sorting, and filtering  
* Check adding/removing products from cart  
* Test checkout process and form validations  
* Verify buttons, links, and navigation

  ### **UI / Visual Testing** {#ui-/-visual-testing}

* Check images, text, buttons, icons, layout, colors, and fonts  
* Verify hover, click, and focus effects

  ### **Negative Testing** {#negative-testing}

* Enter invalid login or form data and check error messages  
* Perform actions that may produce errors

  ### **Usability Testing** {#usability-testing}

* Ensure website is easy to use and intuitive  
* Verify users can complete tasks like login, add to cart, and checkout

  ### **Cross-browser Testing** {#cross-browser-testing}

* Verify site works on Chrome, Firefox, and Edge

  ### **Reporting** {#reporting}

* Record test results in a spreadsheet or document  
* Capture screenshots of defects or errors and prepare bug reports

# 

# Test Scope {#test-scope}

The testing will cover the main features and workflows of Sauce Demo.

## In-scope features {#in-scope-features}

* Login functionality for different types of users

* Product listing and sorting by name and price

* Adding and removing products from the cart

* Checkout process, including filling forms and completing orders

* User interface elements such as buttons, links, and messages

Out-of-scope features:

* Browser compatibility testing

* Security testing

* Performance testing beyond basic observations

This scope ensures that the most important features of the website are tested while keeping the plan simple and manageable.

## 

## 

## 

# Test Objectives {#test-objectives}

The objectives of testing Sauce Demo are:

* To make sure all users can log in and log out correctly

* To verify that products are displayed and sorted correctly by name and price

* To ensure that items can be added to and removed from the cart without errors

* To confirm that the checkout process works and shows correct messages for success or errors

* To check that the website interface behaves as expected and is easy to use

These objectives help guide the testing and ensure that the most important features are working properly.

# Test Environment {#test-environment}

The testing of Sauce Demo will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| Web Browser | Google Chrome, Edge |
| Internet Connection | Stable connection required |
| Device | Desktop , Laptop |
| Operating System | Windows |
| Test Accounts | Provided by Sauce Demo: standard\_user, locked\_out\_user, problem\_user, performance\_glitch\_user, visibillity\_user  |
| Additional Tools  | Browser for manual testing, google sheets for logging test cases and defects |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Writing the test plan document | 1 day  |
| Test Case Design | Creating test cases for login, products, cart, checkout | 1 day |
| Test Environment Setup | Preparing browser, devices, and test accounts | 0.5 day |
| Test Execution – Login | Testing all user login scenarios | 0.5 day |
| Test Execution – Product Page | Testing product display, sorting, and UI elements | 1 day |
| Test Execution – Cart | Adding/removing products and verifying functionality | 0.5 day |
| Test Execution – Checkout | Testing form validation and order completion | 0.5 day |
| Test Reporting | Logging any issues found and summarizing results | 0.5 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for Sauce Demo:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Documentation Tools | Test plan, test cases, bug reporting sheet |
| Reporting Tool | Google Sheets, or any simple tracker |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* Test plan and test cases are ready

* Test environment is set up

* Test accounts are available and working

### **Exit Criteria** {#exit-criteria}

* All planned test cases have been executed

* All critical and major bugs are logged

* Test results are documented

# Test Deliverables {#test-deliverables}

The following items will be produced and used during the testing of Sauce Demo:

* Test plan document

* Test cases document

* Bug/defect report

* Test execution report or summary

* Any screenshots or evidence of testing results

# References / Glossary  {#references-/-glossary}

**References:**

* Sauce Demo website: https://www.saucedemo.com

* Sauce Labs documentation and demo guides

**Glossary:**

* QA: Quality Assurance, the process of ensuring software works correctly

* Test Case: A set of steps to verify a particular feature or functionality

* Bug / Defect: Any issue or error found in the application

* Test Environment: The setup used to perform testing, including browser, device, and accounts

* Test Deliverables: Documents and reports produced during testing

# 

