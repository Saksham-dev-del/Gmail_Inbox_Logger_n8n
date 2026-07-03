\# Gmail Inbox Logger using n8n and Google Sheets



This project automates Gmail inbox tracking using n8n. It fetches unread Gmail messages every 15 minutes, extracts email metadata, appends the data to Google Sheets, and marks processed emails as read.



\## Features



\- Fetches unread Gmail emails automatically

\- Extracts sender name, sender email, subject, preview, label, date, and time

\- Saves email records into Google Sheets

\- Marks processed emails as read

\- Runs every 15 minutes using n8n Schedule Trigger



\## Tech Stack



\- n8n

\- Gmail API

\- Google Sheets API

\- OAuth2

\- Google Sheets

\- Workflow Automation



\## Workflow



```mermaid

flowchart TD

&#x20;   A\[Every 15 Minutes Trigger] --> B\[Get Unread Emails from Gmail]

&#x20;   B --> C\[Format Email Data]

&#x20;   C --> D\[Append Row in Google Sheets]

&#x20;   D --> E\[Mark Email as Read]

&#x20;   E --> F\[Workflow Complete]

