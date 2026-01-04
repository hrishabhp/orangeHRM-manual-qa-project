# 📄 Manual Test Execution Report

## 📊 Requirement Traceability Matrix (RTM)
*Mapping requirements to test scenarios and current execution status.*

| Req ID | Module | Requirement Description | Test Case ID | Status |
| :--- | :--- | :--- | :--- | :--- |
| **REQ-001** | Login | User should be able to login with valid credentials | TC_LOGIN_01 | ✅ PASS |
| **REQ-002** | Login | System should validate invalid credentials | TC_LOGIN_02 | ✅ PASS |
| **REQ-003** | Login | System should validate required fields | TC_LOGIN_03 | ✅ PASS |
| **REQ-004** | Profile | Profile menu should open on click | TC_PROFILE_01 | ✅ PASS |
| **REQ-005** | Profile | **Profile menu should close on toggle click** | **TC_PROFILE_02** | ❌ **FAIL** |
| **REQ-006** | Profile | Profile menu should close on outside click | TC_PROFILE_03 | ✅ PASS |

---

## 🧪 Detailed Test Scenarios

### 🔹 Module 1: Login Functionality

| Test Case ID | Title | Steps | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC_LOGIN_01** | **Verify login with valid credentials** | 1. Open OrangeHRM application<br>2. Enter valid username<br>3. Enter valid password<br>4. Click Login | User should be logged in successfully and redirected to the dashboard. | ✅ PASS |
| **TC_LOGIN_02** | **Verify login with invalid password** | 1. Open OrangeHRM application<br>2. Enter valid username<br>3. Enter invalid password<br>4. Click Login | System should display an appropriate error message "Invalid credentials". | ✅ PASS |
| **TC_LOGIN_03** | **Verify login with empty fields** | 1. Open OrangeHRM application<br>2. Leave username empty<br>3. Leave password empty<br>4. Click Login | System should display validation messages "Required". | ✅ PASS |

### 🔹 Module 2: User Profile & Navigation

| Test Case ID | Title | Steps | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC_PROFILE_01** | **Verify dropdown opens on click** | 1. Login to OrangeHRM<br>2. Click on the user profile icon | Profile dropdown menu should open and display available options. | ✅ PASS |
| **TC_PROFILE_02** | **Verify dropdown toggles closed** | 1. Login to OrangeHRM<br>2. Click icon to open dropdown<br>3. **Click on the same profile icon again** | **Profile dropdown menu should close.** | ❌ **FAIL** |
| **TC_PROFILE_03** | **Verify dropdown closes on outside click** | 1. Open profile dropdown<br>2. Click outside the dropdown area | Profile dropdown menu should close. | ✅ PASS |

---
**Note:** TC_PROFILE_02 failed during execution. Refer to [Issue #1923](https://github.com/orangehrm/orangehrm/issues/1923) for the detailed bug report.