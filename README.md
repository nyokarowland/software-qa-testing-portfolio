# Software QA Testing Portfolio

**Summary:** A fictional QA case study showing how missing validation can affect service-request routing and contact information, with documented defects, root cause analysis, and regression results.

**Project type:** Simulated documentation exercise. The application, execution, defects, corrections, and results are fictional.

## Business Question and Findings

**Question:** Can employees submit complete service requests and maintain valid profile information before the portal is released?

**My role:** I created the test plan, nine functional test cases, two defect reports, a 5 Whys analysis, regression documentation, and a final test summary.

**Findings in the fictional scenario:** The portal accepts a request without a required category and allows an invalid email address to be saved. These gaps could make requests harder to route and prevent reliable follow-up. The documented initial cycle has seven passes and two failures; the simulated correction cycle has six regression passes.

**Recommendation:** Treat required-field and email validation as release checks. Review validation requirements with the development team, retest each correction, and include negative cases in regression coverage. Six passing regression cases cover the selected scope; they do not establish that every application behavior is defect-free.

**Start here:** [Final Test Summary](test-summary/Final-Test-Summary.md) · [Test Cases](test-cases/Test-Cases.md) · [Root Cause Analysis](root-cause-analysis/Root-Cause-Analysis.md)

## Project Overview

This portfolio project demonstrates my approach to software quality assurance and testing. The project is based on a simulated employee service request web application that allows users to log in, submit service requests, review request status, and update account information.

The purpose of this project is to demonstrate how I would evaluate software functionality, document test results, identify defects, perform root cause analysis, and verify corrections through regression testing.

## Project Objectives

- Develop clear and structured test scenarios and test cases
- Compare expected results with actual system behavior
- Identify and document software defects
- Assign defect severity and priority
- Apply root cause analysis techniques
- Document corrective actions
- Perform regression testing after defects are corrected
- Communicate testing results through a final test summary

## Application Under Test

**Application:** Employee Service Request Portal  
**Project Type:** Simulated QA portfolio project

The application allows employees to:

- Log in using authorized credentials
- Submit a new service request
- View existing requests
- Track request status
- Update profile information
- Log out securely

## QA Skills Demonstrated

- Software Quality Assurance
- Manual Testing
- Functional Testing
- Test Case Development
- Defect Reporting
- Regression Testing
- Root Cause Analysis
- 5 Whys Analysis
- Corrective Actions
- Process Improvement
- Documentation
- Expected vs. Actual Results

## Project Documentation

The project documentation follows the QA lifecycle from initial test planning through defect resolution and final regression testing.

- [QA Test Plan](test-plan/QA-Test-Plan.md) — Defines the testing scope, objectives, environment, approach, entry and exit criteria, and defect classification.
- [Test Scenarios and Test Cases](test-cases/Test-Cases.md) — Documents nine functional test cases with test steps, expected results, actual results, and pass/fail status.
- [DEF-001: Missing Required Request Category](defect-reports/DEF-001.md) — Documents the service request validation defect, severity, priority, impact, corrective action, and resolution.
- [DEF-002: Invalid Email Format](defect-reports/DEF-002.md) — Documents the profile email validation defect, impact, corrective action, retesting, and resolution.
- [Root Cause Analysis](root-cause-analysis/Root-Cause-Analysis.md) — Uses the 5 Whys method to analyze DEF-001 and identify corrective and preventive actions.
- [Regression Test Results](regression-testing/Regression-Test-Results.md) — Documents defect retesting and regression testing after corrective actions were applied.
- [Final Test Summary](test-summary/Final-Test-Summary.md) — Summarizes testing results, defect resolution, regression results, and final project status.

## Project Results

| Metric | Result |
|---|---:|
| Initial Test Cases | 9 |
| Initial Passed | 7 |
| Initial Failed | 2 |
| Defects Identified | 2 |
| Defects Resolved | 2 |
| Regression Tests | 6 |
| Regression Tests Passed | 6 |
| Open Defects | 0 |

**Initial Pass Rate:** 77.8%  
**Regression Pass Rate:** 100%

## Project Status

**Complete**

This simulated portfolio project demonstrates the complete QA workflow from test planning and execution through defect reporting, root cause analysis, corrective action, retesting, regression testing, and final reporting.

## About Me

I am an Information Technologies student with professional experience in quality, analytics, operational reporting, and process improvement. My career interests include Software Quality Assurance, Quality Analyst, IT Business and Systems Analysis, Application Support, and technology-focused process improvement roles.
