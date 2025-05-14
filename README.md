📧 GoogleAppScript_email_sender_with_drive_attachment
📋 Overview
This Google Apps Script automates email sending using Gmail based on a structured Google Sheet. Each row contains the recipient’s email address, subject, body, and an optional Google Drive link. If the Drive link is provided, the file will be attached directly to the email—not just included as a link.

✅ Features
Sends emails in batch from a Google Sheet

Supports optional Google Drive file attachments

Marks emails as "Sent" after successful delivery to prevent duplicates

📊 Spreadsheet Structure
Sheet name: EmailQueue

Column	Field Name	Description
A	Email	Recipient's email address
B	Subject	Subject of the email
C	Body	Body content of the email (HTML supported)
D	Drive Link	(Optional) Direct link to file on Google Drive
E	Status	Will be marked as Sent after email is sent

🧰 Setup Instructions
Create a Google Sheet and rename one of the tabs as EmailQueue

In Row 1, set the following headers:
Email | Subject | Body | Drive Link | Status

Fill in email data below those headers

Open Apps Script via Extensions > Apps Script

Paste the script below

Replace or adjust as needed, and run the sendQueuedEmails function
