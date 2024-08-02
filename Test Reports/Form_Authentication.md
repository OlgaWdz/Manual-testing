1. Introduction

This report documents the results of the form authentication testing for the application. The aim was to verify that the authentication mechanism is functioning correctly and securely.

2. Objectives

Ensure that users can successfully log in with valid credentials.
Validate error handling for invalid login attempts.
Verify security measures to protect user data.
Test additional features like "Remember Me" and "Forgot Password."

3. Test Summary

Test Cases Executed: 10
Test Cases Passed: 8
Test Cases Failed: 2
Test Execution Date: 2024-07-30 to 2024-08-01
Test Environment:

Operating System: Windows 10, macOS
Browsers: Google Chrome, Mozilla Firefox, Safari
Devices: Desktop, Mobile

4. Detailed Test Results

Valid Login

Description: Enter valid username and password, click "Login".
Expected Result: Successful login and redirection to homepage.
Actual Result: Passed.
Status: Pass
Invalid Login

Description: Enter invalid username or password, click "Login".
Expected Result: Display appropriate error messages.
Actual Result: Passed.
Status: Pass
Empty Fields

Description: Attempt login with empty username and/or password fields.
Expected Result: Display appropriate error messages.
Actual Result: Passed.
Status: Pass
"Remember Me" Functionality

Description: Check "Remember Me", log in with valid credentials, close and reopen the browser.
Expected Result: User remains logged in.
Actual Result: Failed. User is logged out after reopening the browser.
Status: Fail
"Forgot Password" Functionality

Description: Click "Forgot Password" link.
Expected Result: Redirection to password recovery page.
Actual Result: Passed.
Status: Pass
Password Masking

Description: Ensure password field is masked.
Expected Result: Password characters are not visible.
Actual Result: Passed.
Status: Pass
SQL Injection

Description: Attempt SQL injection in username and password fields.
Expected Result: Application handles it securely.
Actual Result: Passed.
Status: Pass
Brute Force Attack

Description: Simulate multiple login attempts with different passwords.
Expected Result: Account is locked or CAPTCHA is triggered after a set number of failed attempts.
Actual Result: Failed. No account lockout or CAPTCHA triggered.
Status: Fail

5. Defect Summary

"Remember Me" Functionality:

Description: User is logged out after reopening the browser despite selecting "Remember Me".
Severity: Medium
Status: Reported
Brute Force Attack Protection:

Description: No account lockout or CAPTCHA triggered after multiple failed login attempts.
Severity: High
Status: Reported

6. Conclusion

The form authentication testing revealed critical issues with the "Remember Me" functionality and brute force attack protection. These defects have been reported for resolution. Overall, the authentication mechanism functions correctly for valid and invalid login scenarios and other security measures like password masking and SQL injection handling are in place.

