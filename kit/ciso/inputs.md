# CISO inputs

Ask the user for these. Any missing file turns the questions it serves into UNKNOWN.

| File | Where it usually comes from | Serves questions |
|---|---|---|
| Conditional Access policies (JSON) | Microsoft Graph `GET /identity/conditionalAccess/policies`, or your identity provider's policy export | 1, 2 |
| Authentication methods policy (JSON) | Microsoft Graph `GET /policies/authenticationMethodsPolicy`, or your identity provider's equivalent | 1, 4 |
| MDM device inventory (CSV) | Your MDM console's device export | 2, 7 |
| Help desk MFA reset procedure | Your internal runbook | 3 |
| Last three identity incident reports | Your incident tracker (names can be removed first) | 6 |
| Offboarding checklist | HR or IT | 7 |

Fields to skip: device location, app inventories, message content, personal contact details. The method does not need them.
