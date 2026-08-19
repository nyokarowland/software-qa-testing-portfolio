# QA Test Plan

## Project Information

**Project:** Employee Service Request Portal  
**Project Type:** Simulated QA Portfolio Project  
**Testing Type:** Manual Functional Testing  
**Status:** In Progress

## Purpose

The purpose of this test plan is to define the testing approach for the Employee Service Request Portal. Testing will focus on verifying that the application's primary functions operate as expected and that users can complete common tasks without experiencing errors that interfere with system usability.

The testing process will also be used to identify defects, document expected and actual results, evaluate defect severity and priority, and verify corrective actions through regression testing.

## Application Overview

The Employee Service Request Portal is a simulated web application designed to allow employees to manage basic service requests.

Primary application functions include:

- User login
- Service request submission
- Request status tracking
- Viewing existing requests
- Updating user profile information
- Secure logout

## Testing Objectives

The objectives of testing are to:

- Verify that core application functions operate according to expected requirements
- Confirm that valid user information is accepted
- Confirm that invalid or incomplete information is handled appropriately
- Identify functional defects that could affect the user experience
- Document defects using clear reproduction steps
- Evaluate defects based on severity and priority
- Retest corrected defects
- Perform regression testing to verify that corrections do not negatively affect existing functionality

## Scope

### In Scope

The following functionality will be tested:

- Valid user login
- Invalid user login
- Required login fields
- New service request submission
- Required service request fields
- Viewing submitted requests
- Request status display
- Updating profile information
- Logout functionality

### Out of Scope

The following areas are outside the scope of this portfolio project:

- Performance and load testing
- Automated testing
- Penetration testing
- Database performance testing
- Mobile application testing
- Production environment testing

## Testing Approach

Manual functional testing will be used to evaluate the application.

Each test case will include:

- Test case ID
- Test scenario
- Preconditions
- Test steps
- Test data
- Expected result
- Actual result
- Pass or fail status

When a test fails, the issue will be documented as a defect. Defect documentation will include reproduction steps, severity, priority, expected behavior, and actual behavior.

## Test Environment

For purposes of this simulated portfolio project, testing is based on the following environment:

**Application Type:** Web application  
**Operating System:** Windows 11  
**Browser:** Microsoft Edge  
**Test Method:** Manual testing  
**User Type:** Standard employee account

## Entry Criteria

Testing may begin when:

- Application requirements have been identified
- Core application functions are available for testing
- Test scenarios and test cases have been prepared
- Required test data has been identified

## Exit Criteria

Testing will be considered complete when:

- Planned test cases have been executed
- Test results have been documented
- Identified defects have been recorded
- Critical defects have been evaluated
- Corrected defects have been retested
- Regression testing has been completed
- A final test summary has been prepared

## Defect Classification

### Severity

**Critical:** Prevents use of a major application function or creates a serious security or data risk.

**High:** Significantly affects functionality and prevents the user from completing an important task.

**Medium:** Affects functionality but a workaround may be available.

**Low:** Minor issue with limited impact on application functionality.

### Priority

**High:** Should be corrected as soon as possible.

**Medium:** Should be corrected during the normal development cycle.

**Low:** May be corrected in a future update.

## Deliverables

Testing documentation for this project will include:

- QA Test Plan
- Test Scenarios and Test Cases
- Defect Reports
- Root Cause Analysis
- Regression Test Results
- Final Test Summary

## Risks and Considerations

Because this is a simulated portfolio project, the application and test results are designed to demonstrate QA processes rather than represent testing performed on a live production system.

The testing documentation will focus on realistic software quality assurance practices, clear communication, defect identification, and structured problem solving.
