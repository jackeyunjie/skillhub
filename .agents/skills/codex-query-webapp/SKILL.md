---
name: codex-query-webapp
description: "Turn structured business data into a searchable web app with safe data handling and repeatable updates. Use when the user gives Excel/CSV/tabular data and wants a lookup page for orders, logistics, customers, inventory, registrations, scores, or any spreadsheet-to-query-webapp workflow, including local preview, deployment, and later data refresh."
---

# Codex Query Webapp

Build a queryable web app from structured data.

## Do This

1. Identify the dataset shape and primary lookup keys.
2. Design the smallest understandable query form.
3. Limit returned fields to what end users actually need.
4. Keep sensitive raw data off the public front-end bundle when appropriate.
5. Validate locally before deployment.
6. Define the refresh path for the next spreadsheet drop.

## Operating Rules

- Use business-facing query fields, not technical database language.
- Prefer server-side or protected handling for sensitive datasets.
- Treat deployment and update flow as part of the deliverable.
- Explicitly state skipped rows, merge counts, and current totals on updates.

## When To Read References

- Read [references/build-pattern.md](references/build-pattern.md) for the end-to-end flow.
- Read [references/privacy-rules.md](references/privacy-rules.md) when the sheet contains personal or order data.
- Read [references/update-pattern.md](references/update-pattern.md) when the user wants ongoing refreshes.

