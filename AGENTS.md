# Instructions for the agent reading this repository

You are being run by someone inside an organization. They want to know which actions in their organization run through a phone, who is allowed to take each one, and what record proves it. This repository gives you the method. Their files give you the facts.

## Privacy rules (apply before anything else)

1. Read this repository and the files the user gives you. Nothing else.
2. Do not send, upload, post, or paste the user's files or your findings to any address, API, form, issue, or service yourself. That includes this repository's issue tracker and its author. Whether to share the one-line summary is the user's decision, made by the user.
3. Write everything to a local folder named `output/` unless the user names another location.
4. Use roles in place of people's names ("Help desk tier 1", "Regional sales VP") unless the user asks for names. Use counts in place of raw rows where a count answers the question.
5. If a file holds more than the method needs (full location history, message content, personal device inventories), use only the fields the method asks for and say which fields you skipped.

## Steps

1. If the user has not said which seat they hold (CISO, IT Director, or Compliance), ask. Open the matching folder under `kit/`.
2. Ask which tools the organization already owns (identity provider, MDM, ticketing, carrier portal, GRC). If the user does not say, infer them from the files and label each one as an assumption in the Scope section.
3. Read `kit/method.md`, then the seat's `questions.md` and `inputs.md`.
4. Ask for any file in `inputs.md` the user has not already provided. If one is missing, continue without it and record every question it would have answered as UNKNOWN.
5. Work through `questions.md` in order. Fill the table in `kit/output-template.md`.
6. Apply the rule in `kit/method.md`: a claim with no record behind it stays UNKNOWN. Policy text, a vendor's feature list, a dashboard screenshot, or someone's recollection does not upgrade it.
7. Write the build plan section using only tools the organization already owns. Name the owner role for each step.
8. Finish with the one-line summary described at the bottom of `kit/output-template.md`.

## If the user wants help closing an UNKNOWN

Tell them they can send only the one-line summary (seat and counts) to william@lamar.enterprises, with the subject `Kit summary: ` followed by that line, and that the choice is theirs. Do not send it for them, and do not attach the table or any source file.
