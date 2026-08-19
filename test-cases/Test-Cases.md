# Test Scenarios and Test Cases

## Project Information

**Project:** Employee Service Request Portal  
**Project Type:** Simulated QA Portfolio Project  
**Testing Method:** Manual Functional Testing  
**Test Environment:** Windows 11 / Microsoft Edge

## Test Execution Summary

The following test cases were developed to evaluate the primary functions of the simulated Employee Service Request Portal. Results are intentionally designed to demonstrate both successful testing and the identification of defects.

| Test Case ID | Test Scenario | Result |
|---|---|---|
| TC-LOGIN-001 | Login with valid credentials | Pass |
| TC-LOGIN-002 | Login with invalid password | Pass |
| TC-LOGIN-003 | Login with required fields blank | Pass |
| TC-REQ-001 | Submit a valid service request | Pass |
| TC-REQ-002 | Submit request without required category | Fail |
| TC-REQ-003 | View submitted request and status | Pass |
| TC-PROFILE-001 | Update profile with valid information | Pass |
| TC-PROFILE-002 | Enter invalid email format | Fail |
| TC-LOGOUT-001 | Log out of the application | Pass |

---

## TC-LOGIN-001 — Valid User Login

**Test Scenario:** Verify that an authorized user can log in with valid credentials.

**Preconditions:**
- User account exists
- User is on the login page

**Test Data:**
- Username: employee01
- Password: ValidPass123

**Test Steps:**
1. Enter a valid username.
2. Enter a valid password.
3. Select the Login button.

**Expected Result:**  
The user is authenticated and redirected to the employee dashboard.

**Actual Result:**  
The user was successfully authenticated and the employee dashboard displayed.

**Status:** PASS

---

## TC-LOGIN-002 — Invalid Password

**Test Scenario:** Verify that the application prevents login when an incorrect password is entered.

**Preconditions:**
- User account exists
- User is on the login page

**Test Data:**
- Username: employee01
- Password: Incorrect123

**Test Steps:**
1. Enter a valid username.
2. Enter an incorrect password.
3. Select the Login button.

**Expected Result:**  
The application should deny access and display an error message indicating that the credentials are invalid.

**Actual Result:**  
Access was denied and an invalid credentials message displayed.

**Status:** PASS

---

## TC-LOGIN-003 — Required Login Fields

**Test Scenario:** Verify that login cannot continue when required fields are blank.

**Preconditions:**
- User is on the login page

**Test Steps:**
1. Leave the username field blank.
2. Leave the password field blank.
3. Select the Login button.

**Expected Result:**  
The application should prevent login and display validation messages for the required fields.

**Actual Result:**  
Login was prevented and required-field messages displayed.

**Status:** PASS

---

## TC-REQ-001 — Valid Service Request Submission

**Test Scenario:** Verify that a user can submit a service request when all required information is provided.

**Preconditions:**
- User is logged in
- User has access to the New Request page

**Test Data:**
- Category: Hardware
- Subject: Laptop docking station issue
- Description: External monitors are not detected when the laptop is connected to the docking station.

**Test Steps:**
1. Open the New Request page.
2. Select Hardware as the request category.
3. Enter the subject.
4. Enter the request description.
5. Select Submit.

**Expected Result:**  
The request should be saved and a confirmation message and request number should display.

**Actual Result:**  
The request was successfully submitted and a request number displayed.

**Status:** PASS

---

## TC-REQ-002 — Missing Required Request Category

**Test Scenario:** Verify that a service request cannot be submitted without selecting a required category.

**Preconditions:**
- User is logged in
- User is on the New Request page

**Test Data:**
- Category: Blank
- Subject: Unable to access shared folder
- Description: Access to the department shared folder is unavailable.

**Test Steps:**
1. Open the New Request page.
2. Leave the Category field blank.
3. Enter a subject.
4. Enter a description.
5. Select Submit.

**Expected Result:**  
The application should prevent submission and display a message indicating that Category is required.

**Actual Result:**  
The application accepted the request without a category and generated a request number.

**Status:** FAIL

**Related Defect:** DEF-001

---

## TC-REQ-003 — View Request Status

**Test Scenario:** Verify that a user can view the status of a previously submitted request.

**Preconditions:**
- User is logged in
- At least one service request exists

**Test Steps:**
1. Open My Requests.
2. Select an existing request.
3. Review the request details and status.

**Expected Result:**  
The application should display the selected request with its request number, description, category, and current status.

**Actual Result:**  
The request information and current status displayed correctly.

**Status:** PASS

---

## TC-PROFILE-001 — Valid Profile Update

**Test Scenario:** Verify that a user can update profile information using valid data.

**Preconditions:**
- User is logged in
- User is on the Profile page

**Test Data:**
- Email: employee01@example.com
- Phone: 313-555-0148

**Test Steps:**
1. Open the Profile page.
2. Update the email address.
3. Update the phone number.
4. Select Save.

**Expected Result:**  
The updated profile information should be saved and a confirmation message should display.

**Actual Result:**  
The information was saved successfully and a confirmation message displayed.

**Status:** PASS

---

## TC-PROFILE-002 — Invalid Email Format

**Test Scenario:** Verify that the application rejects an improperly formatted email address.

**Preconditions:**
- User is logged in
- User is on the Profile page

**Test Data:**
- Email: employee01example.com

**Test Steps:**
1. Open the Profile page.
2. Replace the current email address with employee01example.com.
3. Select Save.

**Expected Result:**  
The application should reject the email address and display a validation message indicating that a valid email format is required.

**Actual Result:**  
The application accepted and saved the improperly formatted email address.

**Status:** FAIL

**Related Defect:** DEF-002

---

## TC-LOGOUT-001 — User Logout

**Test Scenario:** Verify that a logged-in user can securely log out of the application.

**Preconditions:**
- User is logged in

**Test Steps:**
1. Select the user account menu.
2. Select Logout.
3. Attempt to return to the previous authenticated page.

**Expected Result:**  
The session should end, the login page should display, and authenticated pages should no longer be accessible without logging in again.

**Actual Result:**  
The user was logged out, returned to the login page, and could not access the authenticated page without logging in again.

**Status:** PASS

---

## Test Execution Results

**Total Test Cases:** 9  
**Passed:** 7  
**Failed:** 2

The two failed test cases will be documented as defects and evaluated for severity, priority, root cause, corrective action, and regression testing.

> **Portfolio Note:** The application, test execution, and results documented in this repository are simulated for professional portfolio purposes and are intended to demonstrate software quality assurance processes.
