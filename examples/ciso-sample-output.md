# Sample output (CISO seat)

Fictitious organization. Every name, number, and system state below is invented to show the format.

## 1. Scope

- Seat: CISO
- Files read: Conditional Access policies (exported Sept 2026), authentication methods policy, MDM inventory (Sept 2026), help desk reset runbook v3, three incident reports (Q2 to Q3 2026)
- Files missing: offboarding checklist
- Tools owned: identity provider with Conditional Access, MDM, ticketing tool, carrier business portal (stated by the user)
- Fields skipped for privacy: device location, installed apps

## 2. Actions table

| # | Action | Actor (role) | Conditions required | Proof: system and record | Handoff and owner | Status |
|---|---|---|---|---|---|---|
| 1 | Approve vendor payment over $25k | Finance approver | Compliant device, number-match push | Sign-in log entry with device compliance flag | Identity provider to ERP; ERP owner records approver only | PARTIAL: device state recorded, link to the specific payment is not |
| 2 | Reset MFA after lost phone | Help desk tier 1 | Caller verified by manager callback | None found; runbook requires callback, tickets show no callback field | Help desk to directory; directory team | UNKNOWN |
| 3 | Admin portal sign-in | Global admin | Compliant device, phishing-resistant factor | Conditional Access policy plus sign-in logs | None | PROVEN |
| 4 | Sign-in with SMS code | All staff (legacy group) | None beyond the code | Sign-in logs show method; no record of carrier port-out lock | Carrier to identity provider; no owner named | UNKNOWN |
| 5 | Remove factors on departure | IT operations | Same-day removal | Offboarding checklist not provided | HR to IT; owner unknown | UNKNOWN |

## 3. UNKNOWNs

- **#2:** missing callback record. The ticketing tool could hold it as a required field. Owner: help desk lead.
- **#4:** missing port-out lock record. The carrier business portal can produce it. Owner: none named today.
- **#5:** missing removal record. The identity provider's audit log can show it once the checklist is supplied. Owner: IT operations.

## 4. Build plan

1. Add a required "callback completed by" field to MFA reset tickets in the existing ticketing tool. Owner: help desk lead. Closes #2.
2. Set port-out lock on every company line in the carrier portal and export the confirmation. Owner: IT director. Closes #4.
3. Move the legacy SMS group to the authenticator app using the existing authentication methods policy. Owner: identity team. Reduces #4.
4. Pull 90 days of the identity provider's audit log for departures and match against HR termination dates. Owner: IT operations. Closes #5.

New purchases: none needed.

## 5. One-line summary

`Seat: CISO. Actions reviewed: 5. PROVEN: 1. PARTIAL: 1. UNKNOWN: 3.`
