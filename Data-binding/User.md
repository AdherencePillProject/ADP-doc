# User

## Introduction
User is a object to store data of any acount.

## Attributes
User has following attributes:
1. objectId(unique ID)
2. username
3. password
4. firstname
5. lastname
6. email
7. dateOfBirth
8. emailVerified(whether a user has activated the email[True or False])
9. passwordResettingToken(Used for resetting password)
10. patientPointer(point to the corresponding patient in the Patient table if this user is a patient)
11. doctorPointer(point to the corresponding doctor in the Doctor table if this user is a doctor)

## Verification tests

### Verification setting
Test following cases on login page of web, login activity of Android and objects in database.

### Valid user cases (in database)
| Case   | web | Android |
|--------|-----|---------|
|s@s - s |     |         |
|4@4 - 4 |     |         |
|d@d - d |     |         |
|1@1 - 1 |     |         |
|p@p - p |     |         |
|s@s - s |     |         |

### Invalid user cases (not in database)

| Case   | web | Android |
|--------|-----|---------|
|s@3 - s |     |         |
|4@4 - 3 |     |         |

