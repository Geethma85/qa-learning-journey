## Module Metadata

| Field | Value |
| :--- | :--- |
| **Module Name:** | Login |
| **Test Case ID:** | gfg_01 |
| **Tester Name:** | Geek |
| **Test Case Description:** | To check login functionality of geeksforgeeks website. |
| **Prerequisites:** | 1. Stable internet connection.<br>2. Browser (Chrome, Firefox, internet explorer, etc.) |
| **Tester's Name:** | Geethma |
| **Environmental Information:** | 1. OS: Windows/Linux/Mac<br>2. System: Laptop/Desktop |
| **Test Scenario:** | Checking that after entering the correct username and password, the user can login. |

---

## Test Cases Table

| Test Case ID | Test Scenario | Test Steps | Test Data | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TC_LOGIN_01** | Login with valid credentials | 1. Open login page.<br>2. Enter email and password.<br>3. Click Login. | Valid email and password | User successfully logs in and navigates to the dashboard. | **Pass** |
| **TC_LOGIN_02** | Login with incorrect password | 1. Open login page.<br>2. Enter valid email and incorrect password.<br>3. Click Login. | student@example.com / Wrong@123 | Login is rejected and an appropriate error message is displayed. | **Pass** |
| **TC_LOGIN_03** | Login with unregistered email | 1. Open login page.<br>2. Enter an unregistered email and a password.<br>3. Click Login. | unknown@example.com / Student@123 | Login is rejected and an appropriate error message is displayed. | **Pass** |
| **TC_LOGIN_04** | Login with both fields empty | 1. Open login page.<br>2. Leave both fields empty.<br>3. Click Login. | Email: empty; Password: empty | Required-field validation messages appear, and login is prevented. | **Pass** |
| **TC_LOGIN_05** | Login with empty email | 1. Open login page.<br>2. Enter a password only.<br>3. Click Login. | Email: empty; Password: Student@123 | Email validation message appears, and login is prevented. | **Pass** |
| **TC_LOGIN_06** | Login with empty password | 1. Open login page.<br>2. Enter an email only.<br>3. Click Login. | Email: student@example.com; Password: empty | Password validation message appears, and login is prevented. | **Pass** |
| **TC_LOGIN_07** | Login with invalid email format | 1. Open login page.<br>2. Enter an invalid email format and a password.<br>3. Click Login. | studentexample.com / Student@123 | Email format validation appears, and login is prevented. | **Pass** |
| **TC_LOGIN_08** | Verify password masking | 1. Open login page.<br>2. Enter a password. | Student@123 | Password characters are masked by default. | **Pass** |
| **TC_LOGIN_09** | Verify password case sensitivity | 1. Open login page.<br>2. Enter the correct email and a password with incorrect capitalization.<br>3. Click Login. | student@example.com / student@123 | Login is rejected. | **Pass** |
| **TC_LOGIN_10** | Verify logout and session protection | 1. Log in successfully.<br>2. Log out.<br>3. Try to access the dashboard again. | Valid credentials | The user is logged out and cannot access protected pages without authenticating again. | **Pass** |
