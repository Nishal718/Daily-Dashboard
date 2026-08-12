# Daily Dashboard

This repository contains the maintained prompt and operating checklist for the **My Daily Dashboard** workflow.

The workflow is designed to use connected Gmail, Google Calendar, and Google Drive data to create a mobile-friendly daily dashboard and update it every morning at 8:00 AM local time.

> **Current environment note:** this repository environment does not include authenticated access to Gmail, Google Calendar, Google Drive, Google Sites, or ChatGPT scheduled tasks. Those connections must be approved in the app/runtime where the workflow is executed before the first live run can create or update the Site.

## Required connected apps and permissions

Before running the workflow, connect and approve access to:

- **Gmail**: read-only access to new and unread email, with links to original messages.
- **Google Calendar**: read-only access to events for today and the next seven days.
- **Google Drive**: read-only access to relevant files and file links.
- **Google Sites**: permission to find, create, and update the Site named `My Daily Dashboard`.
- **Scheduled task support**: permission to run the workflow every day at 8:00 AM in the user's local time zone and send a completion notification.

The workflow must not send emails, delete or move files, change calendar events, make purchases, share private information, or perform other external actions unless the user explicitly approves that action.

## Files

- [`daily-dashboard-prompt.md`](daily-dashboard-prompt.md): the production prompt for creating and maintaining the dashboard.
- [`runbook.md`](runbook.md): a concise first-run and scheduled-run checklist.
