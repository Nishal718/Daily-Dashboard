# Daily Dashboard Runbook

## First run

1. Confirm access to Gmail, Google Calendar, Google Drive, Google Sites, and scheduled tasks.
2. If any source is unavailable, stop before dashboard creation and tell the user exactly which connection or permission is missing.
3. Read Google Calendar for today and the next seven days.
4. Read new and unread Gmail messages, filtering for emails that require a reply, include a deadline, involve money or contracts, include bookings or appointments, or require action.
5. Search Google Drive for files connected to today's meetings, current projects, upcoming deadlines, actionable emails, and likely documents needed today.
6. Build the dashboard sections defined in `daily-dashboard-prompt.md`.
7. Search Google Sites for an existing Site named `My Daily Dashboard`.
8. Create the Site only if it does not already exist; otherwise update the existing Site and preserve its URL.
9. Verify the Site can be opened by the authenticated user.
10. Schedule the workflow to run every day at 8:00 AM in the user's local time zone.
11. Report the Site name, Site URL, next scheduled run, and any remaining permission issues.

## Scheduled run

1. Pull fresh Gmail, Calendar, and Drive data.
2. Rebuild the dashboard.
3. Update the existing `My Daily Dashboard` Site without creating a duplicate.
4. Notify the user when the update is complete.
5. Report any source or update failures.

## Privacy and safety

- Do not include full private email bodies or sensitive document contents on the dashboard.
- Use account-protected links whenever possible.
- Do not send emails, delete or move files, change calendar events, make purchases, or share private information without explicit approval.
