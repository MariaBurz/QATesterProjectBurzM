# Final project for ITF Manual Testing Course

The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application.

Application under test: [https://opensource-demo.orangehrmlive.com/](https://opensource-demo.orangehrmlive.com/)

API Documentation: [https://orangehrm.github.io/orangehrm-api-doc/](https://orangehrm.github.io/orangehrm-api-doc/)

The final project will be split into 2 sections: [Testing section]() and [SQL section]().

Tools used: JIRA, Zephyr Squad, Postman, MySQL.

# Functional specifications

1. User Story - User Management Module

![UserStory1](https://user-images.githubusercontent.com/110056890/181301603-fcc322e7-7c75-468c-8a03-0ae87fbcf05a.png)

2. User Story - Job Module

![UserStory2](https://user-images.githubusercontent.com/110056890/181302168-d61ca487-7c2d-452c-a52e-fb23c56b5200.png)

3. User Story - UI 

![UserStory3](https://user-images.githubusercontent.com/110056890/181302276-abe83af7-7b13-4829-ad1e-98b1eef9407e.png)

# 1 Testing section

## 1.1 Test Planning

The Test Plan is designed to describe all details of testing for the X module from the OrangeHRM application.

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan

### 1.1.1 Roles assigned to the project and persons allocated

- Project manager – Pop Ioan
- Product Owner – Popovici Ioana
- Developer – Popescu Ilie
- QA Tester – Burz Maria

### 1.1.2 Entry criteria defined

-	Requirements are approved;
-	The code is ready to be tested;
-	Test cases are defined;
-	Test environment and all the necessary resources are prepared.

### 1.1.3 Exit criteria defined

-	Budget depleted or deadlines meet;
-	Execution of all test cases;
-	All the identified defects are corrected and closed;
-	No critical bug is left out. 

### 1.1.4 Test scope

Tests in scope: All the feature of User Management submenu and Job submenu from Admin Module which were defined in the business requirements and specifications need to be tested: functional testing, GUI testing and API testing.

Tests not in scope: performance testing, integration testing of the Admin Module to other modules, compatibility testing with multiple browsers.

### 1.1.5 Risks detected

Project risks: lack of experience of the QA team, short deadline of Zephyr Squad trial, unavailability of test environment

Product risks: validation constraints on the fields might be too restrictive to the end-user

### 1.1.6 Evaluating entry criteria

The entry criterias defined in the Test Planning phase have been achieved and the test process can continue.

## 1.2 Test Monitoring and Control

Multiple reports were generated. The following report was generated to reflect the current status of the testing process, in case of major problems control measures could be taken. The following status report reflects the proportion of the passed and failed tests. 

![PeriodicReport_Chart](https://user-images.githubusercontent.com/110056890/181305981-817b5db5-f94a-44fa-99a7-14b8425b9d03.png)

## 1.3 Test Analysis

The testing process will be executed based on the above requirements for the Admin Module. The following test conditions were found:

Enter data only for mandatory fields and check that the dependant is created/updated
Enter data for all available fields and check that the dependant is created/updated
Leave mandatory fields empty and check that the dependant cannot be created/updated
View dependant details and check they are correct
View all dependants in a list
Check all validation constraints for the fields



## 1.4 Test Design

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases are:

Test cases:

![JIRA_TestCasesSummary](https://user-images.githubusercontent.com/110056890/181916126-f5345666-8abb-44c1-8026-e5c0c06e5d97.png)

The test cases with steps can be viewed here: [JIRA_TestCases.pdf](https://github.com/MariaBurz/manual_testing_portofolio/blob/main/Final_Project/JIRA_OrangeHRMTestCases.pdf)

For the Dependants API, the following checklist was generated: API_test_checklist.csv

## 1.5 Test Implementation

* Testing environment is up and running: [https://opensource-demo.orangehrmlive.com/](https://opensource-demo.orangehrmlive.com/)
* Access to the testing environment is given: Username : Admin | Password : admin123
* Cycle summary was created
* Test cases were added to the cycle summary
* Postman collection with the dependents API methods was created
* Authorization token was created for accessing the API

## 1.6 Test Execution

Test cases are executed on the created test Cycle summary: Dependents_cycle_summary_execution.pdf
Bugs have been created based on the failed tests. The complete bug reports can be found here: Dependents_created_bugs.pdf
Date format is not dd/mm/yyyy
Future "Date of Birth" can be selected from calendar
Only 50 characters are allowed for "Please Specify" field
Only 50 characters are allowed for "Name" field
Relationship "parent" is missing
API tests are executed based on the checklist. The collection used can be found here: JSON file with the collection of requests created for the Dependents API
Full regression testing is needed after the bugs are fixed

Test cases are executed on the created test Cycle summary: cycle_summary_execution.pdf
Bugs have been created based on the failed tests. The complete bug reports can be found here: created_bugs.pdf
enter here bug titles

## 1.7 Test Completion

![TracebilityMatrix_UserManagementModule](https://user-images.githubusercontent.com/110056890/181340178-b447195e-48e7-47da-9671-e6958d47d526.png)

![TracebilityMatrix_JobModule](https://user-images.githubusercontent.com/110056890/181340216-8688ca18-28e6-4ac4-a349-d7d6d202fe06.png)

![TracebilityMatrix_UserInteraction](https://user-images.githubusercontent.com/110056890/181340251-32b93998-3991-4faa-ba69-822f503e7f3e.png)


As the Exit criteria were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team
The traceability matrix was generated and can be found here: Traceability_matrix.csv
Test execution chart was generated, the final report shows that a number 5 tests have failed of a total of 23
A number of 23 test cases were planned for execution and all of them were executed
A number of 5 total bugs were found, from which the priority is: 1 is high, 4 are medium and 1 is low

Exit criteria was evaluated and passed

The traceability matrix was generated and can be found here: [Traceability_matrix]()

Test execution chart was generated, the final report shows.... -> describe the final report
-> enter here test execution report/chart

# 2 SQL section

In this section I've created a database named 'orangehrm' and  3 tables named 'users', 'job' and 'grade' with all the columns needed to save data per specifications. I've performed different queries inside the sql file: [orangeHRM.sql](https://github.com/MariaBurz/manual_testing_portofolio/blob/main/Final_Project/OrangeHRM.sql)