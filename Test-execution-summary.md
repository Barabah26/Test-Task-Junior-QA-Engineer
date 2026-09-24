# Test Execution Summary

**Scope:** Password field in the Sign Up form only.

**Requirement tested:** Password cannot be shorter than 8 characters.

**Test design techniques used:**

* Equivalence Partitioning
* Boundary Value Analysis
* Positive Testing
* Negative Testing
* Input Validation Testing
* Client/Server Validation Testing

**Test cases executed:** 6

**Passed:** 4

**Failed:** 2

**Defects found:** 1

**Conclusion:**
The password field does not behave according to the specified minimum length requirement. Passwords containing fewer than 8 characters are accepted during registration, including values from the invalid equivalence partition and the 7-character boundary value. A defect was identified: the backend accepts passwords shorter than 8 characters instead of rejecting them.
