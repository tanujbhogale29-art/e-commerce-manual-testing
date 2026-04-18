# 🔐 Test Cases — Login Module

**Module:** Login  
**Tester:** Tanuj Bhogale  
**Date:** March 2026

---

## TC01 — Valid Login

| Field | Details |
|-------|---------|
| **Test Case ID** | TC01 |
| **Module** | Login |
| **Test Case Title** | Login with valid email and password |
| **Type** | Positive |
| **Precondition** | User is registered |
| **Test Steps** | 1. Open login page <br> 2. Enter valid email: `test@gmail.com` <br> 3. Enter valid password: `Test@1234` <br> 4. Click Login button |
| **Expected Result** | User is redirected to homepage/dashboard |
| **Actual Result** | User redirected to homepage ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |

---

## TC02 — Invalid Password

| Field | Details |
|-------|---------|
| **Test Case ID** | TC02 |
| **Module** | Login |
| **Test Case Title** | Login with wrong password |
| **Type** | Negative |
| **Precondition** | User is registered |
| **Test Steps** | 1. Open login page <br> 2. Enter valid email: `test@gmail.com` <br> 3. Enter wrong password: `wrongpass` <br> 4. Click Login button |
| **Expected Result** | Error message: "Invalid email or password" |
| **Actual Result** | No error message shown, page reloads ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-001](../bug-reports/BUG-001.md) |

---

## TC03 — Empty Fields

| Field | Details |
|-------|---------|
| **Test Case ID** | TC03 |
| **Module** | Login |
| **Test Case Title** | Login with empty email and password fields |
| **Type** | Negative |
| **Precondition** | None |
| **Test Steps** | 1. Open login page <br> 2. Leave email and password blank <br> 3. Click Login button |
| **Expected Result** | Validation error: "Fields cannot be empty" |
| **Actual Result** | Login accepted blank spaces as input ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-002](../bug-reports/BUG-002.md) |

---

## TC04 — Max Character Password

| Field | Details |
|-------|---------|
| **Test Case ID** | TC04 |
| **Module** | Login |
| **Test Case Title** | Login with password at max character boundary (50 chars) |
| **Type** | Boundary |
| **Precondition** | User registered with 50-char password |
| **Test Steps** | 1. Open login page <br> 2. Enter email <br> 3. Enter 50-character password <br> 4. Click Login |
| **Expected Result** | Login successful (50 chars is valid boundary) |
| **Actual Result** | Login successful ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |
