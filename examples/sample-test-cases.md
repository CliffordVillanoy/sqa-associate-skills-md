# Sample Test Cases

## Test Case 1: Valid Login

Summary: Verify successful login with valid credentials

Preconditions:

* User account is registered

Steps:

1. Navigate to login page
2. Enter valid username and password
3. Click login

Expected Result:

* User is redirected to dashboard

---

## Test Case 2: Invalid Password

Summary: Verify login fails with incorrect password

Steps:

1. Enter valid username
2. Enter invalid password
3. Click login

Expected Result:

* Error message is displayed

---

## Test Case 3: Boundary Input Validation

Summary: Verify input field boundary validation (1–100)

Steps:

1. Enter value 0
2. Enter value 1
3. Enter value 100
4. Enter value 101

Expected Result:

* 1 and 100 accepted
* 0 and 101 rejected
