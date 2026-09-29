# Output template

Write the result to `output/phone-actions.md` using this layout.

## 1. Scope

- Seat:
- Files read (name and date range):
- Files missing:
- Tools owned (stated by the user, or marked as assumed):
- Fields skipped for privacy:

## 2. Actions table

| # | Action | Actor (role) | Conditions required | Proof: system and record | Handoff and owner | Status |
|---|---|---|---|---|---|---|
| 1 | | | | | | PROVEN / PARTIAL / UNKNOWN |

- **PROVEN:** a record shows the conditions were true when the action happened.
- **PARTIAL:** a record exists for some conditions and not others. Say which.
- **UNKNOWN:** no record found.

## 3. UNKNOWNs

For each UNKNOWN: the action, the missing record, the system that could produce it (or "none yet"), and the owner role.

## 4. Build plan

Numbered steps. Each step names the tool the organization already owns, the owner role, and which UNKNOWN it closes. Keep new purchases in a separate list at the end, with the reason an owned tool cannot do it.

## 5. One-line summary

`Seat: <seat>. Actions reviewed: <n>. PROVEN: <n>. PARTIAL: <n>. UNKNOWN: <n>.`

This line holds counts only: no organization name, no people, no systems. It is the only part of the result meant to leave the organization, and only if the user chooses to send it.
