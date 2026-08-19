# Regression Test Results

## Project Information

**Project:** Employee Service Request Portal  
**Project Type:** Simulated QA Portfolio Project  
**Testing Method:** Manual Functional and Regression Testing  
**Environment:** Windows 11 / Microsoft Edge  
**Related Defects:** DEF-001 and DEF-002

## Purpose

The purpose of regression testing is to verify that corrective actions for identified defects resolved the reported issues without negatively affecting previously working application functionality.

The two failed test cases, TC-REQ-002 and TC-PROFILE-002, were retested after simulated corrections were applied. Related functionality was also tested to confirm that the changes did not introduce additional defects.

## Corrective Actions Tested

### DEF-001 — Missing Required Request Category

Validation was added to prevent a service request from being submitted when the Category field is blank.

### DEF-002 — Invalid Email Format

Email-format validation was added to prevent improperly formatted email addresses from being saved in the user profile.

---

## Defect Retest Results

| Test Case ID | Related Defect | Retest Scenario | Expected Result | Retest Result |
|---|---|---|---|---|
| TC-REQ-002 | DEF-001 | Submit request without required category | Submission is blocked and required-field message displays | Pass |
| TC-PROFILE-002 | DEF-002 | Save profile with invalid email format | Invalid email is rejected and validation message displays | Pass |

---

## DEF-001 Retest

### Test Case

**TC-REQ-002 — Missing Required Request Category**

### Retest Steps

1. Log into the Employee Service Request Portal.
2. Open the New Request page.
3. Leave the Category field blank.
4. Enter a valid subject.
5. Enter a valid description.
6. Select Submit.

### Expected Result

The application should prevent submission and display a message indicating that Category is required.

### Actual Result

The application prevented the request from being submitted and displayed a required-field validation message for Category.

**Retest Status:** PASS

**Defect Status:** Resolved

---

## DEF-002 Retest

### Test Case

**TC-PROFILE-002 — Invalid Email Format**

### Retest Steps

1. Log into the Employee Service Request Portal.
2. Open the Profile page.
3. Enter an improperly formatted email address.
4. Select Save.

### Expected Result

The application should reject the invalid email address and display a message indicating that a valid email format is required.

### Actual Result

The application rejected the invalid email address and displayed an email-format validation message.

**Retest Status:** PASS

**Defect Status:** Resolved

---

## Regression Test Execution

Related application functions were retested after the corrections were applied.

| Test Case ID | Regression Scenario | Result |
|---|---|---|
| TC-REQ-001 | Submit valid service request | Pass |
| TC-REQ-002 | Required category validation | Pass |
| TC-REQ-003 | View request status | Pass |
| TC-PROFILE-001 | Save valid profile information | Pass |
| TC-PROFILE-002 | Invalid email validation | Pass |
| TC-LOGOUT-001 | Secure user logout | Pass |

## Regression Results Summary

**Regression Tests Executed:** 6  
**Passed:** 6  
**Failed:** 0

No new defects were identified during regression testing.

The corrective actions successfully resolved DEF-001 and DEF-002 while related service request, profile, and logout functionality continued to operate as expected.

## Conclusion

Regression testing confirmed that the implemented corrections addressed the identified validation defects without negatively affecting the related application functions included in the regression test scope.

Both previously failed test cases passed during retesting, and all selected regression test cases completed successfully.

> **Portfolio Note:** The application, corrective actions, retesting, and regression results documented in this repository are simulated for professional portfolio purposes and are intended to demonstrate software quality assurance practices.
