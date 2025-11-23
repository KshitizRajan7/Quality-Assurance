# Sauce Demo Automation Test plan

# 

Author : Kshitiz Rajan

# Table of Content

[**Introduction	3**](#introduction)

[Purpose	3](#purpose)

[Overview of the application	3](#overview-of-the-application)

[Audience	3](#audience)

[**Test Strategy / Approach	4**](#test-strategy-/-approach)

[Automation Tool	4](#automation-tool)

[Functional Testing	4](#functional-testing)

[UI / Visual Testing	4](#ui-/-visual-testing)

[Negative Testing	4](#negative-testing)

[Reusability and Maintenance	4](#reusability-and-maintenance)

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

This automation test plan is prepared for Sauce Demo, a sample e-commerce website provided by Sauce Labs. The plan focuses on automating repetitive and critical test cases to save time and improve testing efficiency. Automation will cover features like login, product sorting, cart operations, and checkout.

# Purpose  {#purpose}

The purpose of this automation test plan is to:

* Automate repetitive test cases for faster execution

* Ensure critical functionalities work correctly after every change

* Reduce manual effort and human errors

* Provide quick feedback on website stability

# Overview of the application {#overview-of-the-application}

Sauce Demo is a sample e-commerce website used for practicing automation testing. Users can log in, view products, sort them by name or price, add items to the cart, and complete the checkout process.

The automation test plan focuses on creating scripts to automatically test the most important features, such as login, product sorting, cart operations, and checkout. This helps save time, reduces manual effort, and ensures the website works correctly after changes.

# Audience	 {#audience}

This automation test plan is intended for the QA tester (you) who will create, execute, and maintain automation scripts for Sauce Demo.

It can also be useful for anyone reviewing or understanding the automation testing approach, such as developers or future testers.

# Test Strategy / Approach {#test-strategy-/-approach}

The automation testing of Sauce Demo using Cypress will follow these steps:

### **Automation Tool** {#automation-tool}

* Use **Cypress** for creating scripts

### **Functional Testing** {#functional-testing}

* Automate login and logout tests with valid and invalid credentials  
* Automate product listing, sorting, and filtering tests  
* Automate adding products to the cart and removing them  
* Automate checkout process and form validations  
* Automate verification of buttons, links, and navigation

### **UI / Visual Testing** {#ui-/-visual-testing}

* Automate verification of visible elements like images, text, buttons, and icons  
* Check layout, colors, fonts, and alignment automatically  
* Verify click, and focus effects as part of automation

### **Negative Testing** {#negative-testing}

* Automate tests with invalid login credentials  
* Automate form submission with invalid or empty data  
* Verify error messages and alerts are displayed correctly

### **Reusability and Maintenance** {#reusability-and-maintenance}

* Create reusable test scripts for common actions (login, add to cart, checkout)  
* Use fixtures or test data files for multiple input data  
* Organize scripts for easy maintenance and updates

### **Reporting** {#reporting}

* Generate automated test reports with pass/fail status  
* Capture screenshots for failed tests

# Test Scope {#test-scope}

The automation testing will cover the main features and workflows of Sauce Demo:

* Login functionality for all user types (standard, locked-out, problem, performance glitch)

* Product listing and sorting by name and price

* Adding and removing products from the cart

* Checkout process, including form validation and order completion

* User interface elements like buttons, links, and messages

**Out of scope:**

* Browser compatibility testing beyond default Cypress-supported browsers

* Security testing

* Performance testing beyond basic automation checks

This scope ensures that the most important functionalities are automated while keeping the plan manageable.

## 

## 

## 

# Test Objectives {#test-objectives}

The objectives of automation testing Sauce Demo are:

* Automate login scenarios for all user types to verify correct behavior

* Ensure products are displayed and sorted correctly by name and price

* Automate adding and removing items from the cart to confirm functionality

* Validate the checkout process automatically, including form fields and order completion

* Check that key user interface elements work as expected through automation

* Generate automated test reports to track results and issues efficiently

These objectives guide the automation effort to ensure that critical workflows of Sauce Demo are tested reliably and efficiently.

# Test Environment {#test-environment}

The testing of Sauce Demo will be done in a simple setup using:

| Environment Items | Description |
| :---- | :---- |
| Web Browser | Google Chrome, Edge |
| Internet Connection | Stable connection required |
| Device | Desktop , Laptop |
| Test Accounts | Provided by Sauce Demo: standard\_user, locked\_out\_user, problem\_user, performance\_glitch\_user, visibillity\_user  |
| Automation Tools  | Cypress (installed via Node.js) , VS Code |
| Dependencies | Cypress Drivers,Node.js, required Npm packages  |
| Operating System  | Windows |

# Test Schedule {#test-schedule}

| Testing Activity | Description | Estimated Time |
| ----- | ----- | ----- |
| Test Plan Preparation | Writing the automation test plan | 1 day  |
| Test Case Design | Installing Cypress, setting up test accounts and dependencies | 0.5 day |
| Automation Script Design | Creating scripts for login, product sorting, cart, and checkout | 1 day |
| Test Execution – Login | Running automated login tests for all user types | 0.5 day |
| Test Execution – Product Page | Running automated tests for product display and sorting | 0.5 day |
| Test Execution – Cart | Running automated tests for adding/removing products | 0.5 day |
| Test Execution – Checkout |  Running automated tests for checkout process and form validation  | 0.5 day |
| Test Reporting | Reviewing automated test results, logging any issues, and generating reports | 0.5 day |

# Test Resources {#test-resources}

The following resources will be used to plan, execute, and track the testing activities for Sauce Demo:

| Resource Type | Description |
| ----- | ----- |
| Tester | QA tester |
| Automation Tool | Cypress |
| Test Data | Fixtures or Json files used in automation scripts |
| Documentation Tools | Test plan, test cases, bug reporting sheet |
| Reporting Tool | Cypress built-in reporter or any external reporter for logs and results |

# Entry/Exit Criteria {#entry/exit-criteria}

### **Entry Criteria** {#entry-criteria}

* Cypress is installed and set up

* Test environment is ready

* Test accounts are available and working

* Automation test cases are prepared

* Required test data (fixtures) is available

  ### **Exit Criteria** {#exit-criteria}

* All planned automated test cases have been executed

* All critical and major issues found during automation are logged

* Test results and reports are generated

* Scripts are updated or fixed if any failures are due to script issues


# Test Deliverables {#test-deliverables}

The following items will be produced and used during the automation testing of Sauce Demo:

* Automation test plan document

* Automation test scripts (Cypress)

* Cypress configuration and project setup files

* Test data files (fixtures) used for automation

* Automated test execution report

* Screenshots and videos captured by Cypress during test runs

* Defect report for bugs found through automation

* Final automation summary report


# References / Glossary  {#references-/-glossary}

### **References** {#references}

* Sauce Demo website (test application)

* Cypress official documentation

* JavaScript documentation

* Automation testing best practices

  ### **Glossary** {#glossary}

* **Automation Testing** – Running tests using scripts instead of manual steps.

* **Cypress** – A JavaScript-based automation testing framework for web applications.

* **Test Script** – Code written to automate a test case.

* **Fixture** – Test data file used during automated testing.

* **Test Runner** – The tool that executes test scripts (Cypress Test Runner).

* **Assertion** – A validation step that checks if the result is correct.

* **CI/CD** – Continuous Integration / Continuous Delivery pipeline used to run tests automatically.

* **DOM** – Document Object Model; structure of a web page Cypress interacts with.

* **Selector** – A way to locate an element on a webpage (e.g., CSS selector).

* **Report** – The output showing which tests passed or failed.




# 

