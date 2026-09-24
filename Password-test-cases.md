# Password Test Cases

---

## TC-Password-01

**Test Case:**
Verify that an empty password is not accepted.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
https://www.demoblaze.com/

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Leave the password field empty.
4. Submit the registration form.

**Expected Result:**
The password is not accepted and a validation error is displayed.

**Type:** Negative
**Priority:** High

---

## TC-Password-02

**Test Case:**
Verify that a password containing fewer than 8 characters is rejected.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
Password: `123456`

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Enter `123456` in the password field.
4. Submit the registration form.

**Expected Result:**
The password is rejected and a validation error is displayed.

**Type:** Negative
**Priority:** High

---

## TC-Password-03

**Test Case:**
Verify that a password containing exactly 7 characters is rejected.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
Password: `1234567`

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Enter `1234567` in the password field.
4. Submit the registration form.

**Expected Result:**
The password is rejected and a validation error is displayed.

**Type:** Negative
**Priority:** High

---

## TC-Password-04

**Test Case:**
Verify that a password containing exactly 8 characters is accepted.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
Password: `12345678`

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Enter `12345678` in the password field.
4. Submit the registration form.

**Expected Result:**
The password is accepted and no password validation error is displayed.

**Type:** Positive
**Priority:** High

---

## TC-Password-05

**Test Case:**
Verify that a password containing 9 characters is accepted.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
Password: `123456789`

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Enter `123456789` in the password field.
4. Submit the registration form.

**Expected Result:**
The password is accepted and no password validation error is displayed.

**Type:** Positive
**Priority:** High

---

## TC-Password-06

**Test Case:**
Verify that character composition does not affect password validation when the password length is 8 or more characters.

**Precondition:**
User is on the Sign Up form.

**Test Data:**
Password: `2dsad!@.`

**Steps:**

1. Open the Sign Up form.
2. Enter a valid username.
3. Enter `2dsad!@.` in the password field.
4. Submit the registration form.

**Expected Result:**
The password is accepted and no password validation error is displayed, since no character-type restrictions are specified.

**Type:** Positive
**Priority:** Medium

---
