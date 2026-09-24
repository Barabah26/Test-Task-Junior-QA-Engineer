**Password length validation**

* Verify that an empty password is not accepted;
* Verify that a password containing fewer than 8 characters is rejected;
* Verify that a password containing exactly 7 characters is rejected;
* Verify that a password containing exactly 8 characters is accepted;
* Verify that a password containing 9 characters is accepted;
* Verify that passwords from the invalid equivalence partition (< 8) are rejected;
* Verify that passwords from the valid equivalence partition (≥ 8) are accepted;
* Verify that character composition does not affect validation when the password length satisfies the requirement, since no character-type restrictions are specified;
* Inspect the network request for an invalid password and verify whether validation is performed on the frontend, backend, or both.
