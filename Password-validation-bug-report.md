# Bug Report

## Summary

Passwords shorter than 8 characters are accepted during sign-up.

## Environment

* **Website:** Demoblaze
* **Browser:** Google Chrome
* **OS:** Windows 11

## Preconditions

User is on the Sign Up form.

## Reproduction Steps

1. Open the Demoblaze website.
2. Open the Sign Up form.
3. Enter a valid username.
4. Enter `1234567` into the Password field.
5. Submit the registration form.
6. Observe the result.

## Test Data

`1234567`

## Expected Result

The password should be rejected because the requirement states that a password cannot be shorter than 8 characters. Registration should not be successfully completed.

## Actual Result

The 7-character password is accepted, and the registration is successfully completed.

## Severity

**Medium**

## Priority

**High**

## Root cause

The registration request containing a 7-character password was sent to the API. The API returned **HTTP 200** instead of rejecting the invalid password. This indicates that the minimum password length requirement is not enforced by the backend.

## Suggested Fix

Add server-side validation to reject passwords shorter than 8 characters during registration.

## Responsible Team

**Backend Team**

## Attachments

### API Request

The following request was sent to the API:

![API request](https://github.com/user-attachments/assets/adbc302a-2f4a-44a3-b3da-6892a0247da4)

### API Response

The API returned **HTTP 200** and accepted the registration request:

![API response](https://github.com/user-attachments/assets/aea63d3d-7bbf-4408-aa97-53619ad7a791)

### Video Recording

[Watch the video recording](https://www.awesomescreenshot.com/video/56821783?key=3f03847ed973b576666dd616be44542b)
