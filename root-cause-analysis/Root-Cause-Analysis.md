# Root Cause Analysis

## Project Information

**Project:** Employee Service Request Portal  
**Project Type:** Simulated QA Portfolio Project  
**Related Defect:** DEF-001  
**Related Test Case:** TC-REQ-002  
**Analysis Method:** 5 Whys

## Problem Statement

The Employee Service Request Portal allows a user to submit a service request without selecting a required Category.

Although the Category field is defined as required, the application accepts the request, creates a request number, and stores the request without category information.

## Business Impact

Missing category information may affect:

- Service request routing
- Assignment to the appropriate support team
- Operational reporting
- Request classification
- Data quality
- Resolution efficiency

## 5 Whys Analysis

### Why 1

**Why was the service request submitted without a category?**

The application allowed the Submit action to continue even though the Category field was blank.

### Why 2

**Why did the application allow submission with a blank Category field?**

Required-field validation was not being enforced for the Category field during form submission.

### Why 3

**Why was required-field validation not enforced?**

The Category field was displayed as required in the user interface, but the submission logic did not contain the corresponding validation rule.

### Why 4

**Why was the validation rule missing from the submission logic?**

The functional requirement for Category validation was not fully translated into the form validation implementation.

### Why 5

**Why was the missing validation not identified before testing?**

The development and review process did not include a validation checklist confirming that all required fields had corresponding enforcement rules before the feature was released for QA testing.

## Root Cause

The identified root cause is a gap between the documented field requirement and the implemented form validation logic.

The Category field was identified as required, but the requirement was not consistently enforced within the application. The review process also lacked a structured validation check that could have identified the missing rule earlier.

## Corrective Action

The immediate corrective action is to add validation to the Category field so that:

- A category must be selected before the request can be submitted
- The application prevents submission when Category is blank
- A clear required-field message is displayed
- No incomplete request record is created

## Preventive Action

To reduce the likelihood of similar defects in future development:

- Add required-field validation checks to development review criteria
- Include positive and negative validation scenarios in test planning
- Review form requirements against implemented validation rules
- Include required-field verification in regression testing
- Use a standard checklist for forms containing mandatory fields

## Verification Plan

After the correction is implemented:

1. Re-execute TC-REQ-002.
2. Confirm that a request cannot be submitted with a blank Category.
3. Confirm that the required-field validation message displays.
4. Execute TC-REQ-001 to verify that valid requests can still be submitted.
5. Test other required fields for similar validation issues.
6. Perform regression testing on the service request workflow.

## Expected Outcome

After corrective action is completed, users should be unable to submit incomplete service requests when Category is required.

The additional preventive controls should also improve consistency between documented requirements, development implementation, and QA validation.

> **Portfolio Note:** This root cause analysis is part of a simulated QA portfolio project. The application, defect, root cause, and corrective actions are fictional and are intended to demonstrate quality assurance and structured problem-solving techniques.
