# Update Pattern

When a new spreadsheet arrives:

1. Read the new rows.
2. Merge against existing records.
3. Skip blank or invalid rows.
4. Report:
   - old total
   - rows read
   - rows added
   - rows skipped
   - new total
5. Rebuild and redeploy if requested.

