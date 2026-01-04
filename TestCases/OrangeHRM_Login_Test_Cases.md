# OrangeHRM – Login Module Test Cases

## Test Case ID: TC_LOGIN_01
**Title:** Verify login with valid credentials  
**Precondition:** User is registered and active  

**Steps:**
1. Open OrangeHRM application
2. Enter valid username
3. Enter valid password
4. Click Login

**Expected Result:**  
User should be logged in successfully and redirected to the dashboard.

---

## Test Case ID: TC_LOGIN_02
**Title:** Verify login with invalid password  

**Steps:**
1. Open OrangeHRM application
2. Enter valid username
3. Enter invalid password
4. Click Login

**Expected Result:**  
System should display an appropriate error message.

---

## Test Case ID: TC_LOGIN_03
**Title:** Verify login with empty username and password  

**Steps:**
1. Open OrangeHRM application
2. Leave username field empty
3. Leave password field empty
4. Click Login

**Expected Result:**  
System should display validation messages for required fields.
