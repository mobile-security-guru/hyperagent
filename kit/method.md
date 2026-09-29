# Method

Every row in the output answers the same six questions about one action.

1. **Action.** What business action happens on or through a phone? Name it the way the business names it: approve a payment, reset a password, sign a patient note, change a payout account, grant admin access.
2. **Actor.** Which role is allowed to take it?
3. **Conditions.** Under which current conditions? Device state, location, time, ticket, approval, employment status.
4. **Proof.** Which system holds a record that the conditions were true when the action happened? Name the system and the record.
5. **Handoff.** Where does the action cross from one system or owner to another (carrier to identity provider, help desk to directory, HR to access)? Who owns the result on the other side?
6. **Gap.** Where the answer to 4 or 5 is missing, write UNKNOWN.

## The rule

A claim with no record behind it stays UNKNOWN.

These do not count as a record on their own:

- a policy that says the control exists
- a purchased license or an enabled feature
- a dashboard that shows the state it was built to measure, when the action needs a different state
- a vendor statement
- someone's recollection

They can point you to where a record should be. Go look for it.

## What good looks like

- Each action has one owner role.
- Each handoff has an owner on both sides.
- Each UNKNOWN has a named system that could close it, or says none exists yet.
- The build plan uses tools the organization already pays for before it suggests anything new.
