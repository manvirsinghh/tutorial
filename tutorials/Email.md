## Email Module

The Email module is typically used for sending and receiving emails. It allows you to manage email configurations, templates, and email notifications in your Frappe application.

### Email Doctypes Details:

#### 1. Email Account

The **Email Account Doctype** is used to configure email accounts for sending and receiving emails from within the Frappe system.

**Fields**:
- **Email ID**: The email address associated with the account (e.g., example@gmail.com).
- **SMTP Server**: The outgoing mail server (e.g., smtp.gmail.com).
- **SMTP Port**: The port for SMTP (e.g., 587 for Gmail).
- **SMTP SSL/TLS**: Option to enable SSL/TLS encryption for the outgoing mail server.
- **Incoming Mail Server**: The IMAP or POP server for receiving emails (e.g., imap.gmail.com for Gmail).
- **Incoming Mail Port**: The port for the incoming mail server (e.g., 993 for IMAP).
- **Authentication**: Credentials to authenticate the email account (username and password).
- **Use Outgoing Server**: Option to use the configured SMTP server for sending emails.
- **Email Settings**: Further settings like "use outgoing mail server" and whether to check for incoming mail.

**Purpose**:
- Allows the system to send emails via an SMTP server.


#### 2. Email Template

The **Email Template Doctype** is used to create reusable email templates. These templates can contain dynamic fields (placeholders) that can be replaced with actual data when sending emails.

**Fields**:
- **Name**: The name of the template (e.g., "Welcome Email").
- **Subject**: The subject line of the email.
- **Message**: The body content of the email
- **Is Standard**: Option to mark this template as a standard template for reuse.

**Purpose**:
- Used to standardize and reuse email formats (e.g., for welcome emails, notifications, etc.).


#### 3. Email Queue

The **Email Queue Doctype** keeps track of emails that are scheduled to be sent. It helps in managing and monitoring the status of emails being processed in the background.

**Fields**:
- **Subject**: The subject of the email.
- **Recipients**: The email addresses of the recipients.
- **Status**: The current status of the email (e.g., "Queued," "Sent," or "Failed").
- **Message**: The body content of the email.
- **Sent By**: The user who sent the email.
- **Scheduled Date**: The scheduled time for sending the email.
- **Reference Document**: The reference to the document or task related to the email.

**Purpose**:
- Used to queue and track emails that are being sent 
- Keeps an eye on whether an email was sent successfully or failed.

#### 4. Notification

The **Notification Doctype** is used to define rules for automatic email notifications based on certain events or document states.

**Fields**:
- **Name**: The name of the notification rule.
- **Document Type**: The type of document for which the notification is triggered (e.g., "Sales Order," "Lead").
- **Condition**: The condition to check (e.g., when a document is created, updated, or meets a certain criteria).
- **Message**: The email body, which can be a predefined template or custom message.
- **Email Template**: The email template used for the notification.
- **Recipients**: The users or email addresses to whom the email will be sent.
- **Send on Event**: Defines when the notification should be triggered (e.g., when the document is created, on status change).

**Purpose**:
- Allows automatic email notifications when certain conditions are met for specific documents.
- Helps to send reminders, alerts, or confirmations based on events.

#### 5. Email Domain

The **Email Domain Doctype** is used for configuring the domain to be used for sending email, particularly for emails sent from Frappe's built-in email server.

**Fields**:
- **Name**: The name of the email domain.
- **Domain**: The domain name used for sending emails (e.g., example.com).
- **SMTP Server**: The SMTP server associated with the domain.
- **SMTP Port**: The port used for sending emails (usually 587 or 465).
- **SSL**: Whether SSL encryption is enabled for the server.

**Purpose**:
- Allows Frappe to use a specific domain for sending emails.
- Ensures proper domain configuration for SMTP servers.

#### 6. Email Settings

The **Email Settings Doctype** is where you configure global email-related settings for your Frappe application, such as default SMTP configurations and sending limits.

**Fields**:
- **Default Email**: The default "From" email address to use when sending emails.
- **Default SMTP Server**: The default SMTP server to use for sending emails.
- **SMTP Port**: The default port for sending emails.
- **Use Default Settings**: Option to use the default email configuration across the system.
- **Send Email for User**: Whether to send an email when a user is created, reset, etc.

**Purpose**:
- Centralized location for managing email settings that apply globally across Frappe.

#### 7. Email Digest

The **Email Digest Doctype** is used for creating email digests (periodic emails that summarize activities). This is often used for daily or weekly activity summaries.

**Fields**:
- **Name**: The name of the email digest.
- **Frequency**: How often the digest should be sent (e.g., daily, weekly).
- **Recipients**: The users who should receive the email digest.
- **Subject**: The subject of the digest email.
- **Content**: The content to include in the email digest.

**Purpose**:
- Allows for scheduled, periodic emails that summarize activities or updates (e.g., daily reports or weekly summaries).
