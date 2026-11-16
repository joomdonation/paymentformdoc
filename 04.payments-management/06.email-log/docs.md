---
title: 'Emails Log'
taxonomy:
    category:
        - docs
---

Use **Emails Log** to check which address Payment Form tried to email and what the message contained. To record new entries, set **Log Emails** to **Yes** in **Components → Payment Form → Configuration → General**.

## Find a payment email

1. Go to **Components → Payment Form → Emails Log**.
2. Use **Sent To** to filter by **User** or **Admin**. Use **Email Type** to narrow the list to a category such as **New Payment Email** or **Payment Approved Email**.
3. Click the email subject to review the recipient, timestamp, and message body.

A log entry records a send attempt. If the recipient did not receive the message, check the logged address, the recipient's spam folder, and Joomla's mail settings. Send a test email using Joomla's Global Configuration to check whether your site can send mail.

If you find no entry, check that logging was enabled and that the payment reached the status that triggers the email. Review the subject, body, and recipient settings for the form and the [default messages](/getting-started/configuration/messages). To send the standard payment emails again, see [Resend Email](/payments-management/resend-email).

## Remove entries

Select entries and click **Delete** to remove them from the log. **Delete All** clears the entire log, even when a filter is active. To keep recent entries and remove older ones automatically, set up the [Clean Emails Log](/scheduled-tasks/clean-emails-log) task.
