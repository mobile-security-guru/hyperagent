# IT Director inputs

Ask the user for these. Any missing file turns the questions it serves into UNKNOWN.

| File | Where it usually comes from | Serves questions |
|---|---|---|
| MDM device inventory (CSV) | Your MDM console's device export | 1, 2, 6 |
| Carrier invoice or line detail (CSV or PDF) | Your carrier's business portal | 1, 5 |
| Carrier account authorized users | Your carrier's business portal, account settings | 4 |
| Help desk tickets, last 90 days (CSV) | Your ticketing tool, filtered for: new phone, lost phone, reset, MFA, authenticator, number, SIM, port | 2, 3 |
| MDM device action history (optional) | Your MDM console's audit or device action log (wipe, retire, enroll) | 2 |
| Sign-in device summary (counts) | Your identity provider's sign-in logs, grouped by managed or unmanaged device | 6 |

Fields to skip: call and data usage detail, location, app inventories, personal contact details. The method does not need them.
