Title: Incorrect Authentication Error Message on Login Form

Description: When a user enters an invalid username or password, the login form displays a generic error message instead of a specific message indicating whether the username or password is incorrect.

Steps to Reproduce:

1. Go to the login page at `https://the-internet.herokuapp.com/login`.
2. Enter an invalid username (e.g., `invalidUser`) and a valid password.
3. Click on the "Login" button.
4. Observe the error message displayed.

Expected Result: The system
should
display an error message indicating that the username is incorrect.

Actual Result: The system displays a generic error message: "Invalid login credentials."

Severity: Medium

Priority: High

Environment:

- Operating System: Windows 10
- Browser: Google Chrome, Version 91.0.4472.124
- Device: Desktop

Attachments:

- Screenshot: [Error_Message.png](#)
- Logs: [Login_Logs.txt](#)
Additional Information:

- The issue does not occur when an invalid password is entered with a valid username. In that case, the error message correctly indicates that the password is incorrect.
- Similar behavior is observed on Mozilla Firefox and Microsoft Edge.

Reported by: [Your Name]

Date:2024-08-02

Status: Open