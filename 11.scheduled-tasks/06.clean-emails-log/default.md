---
title: 'Clean Emails Log'
media_order: task-paymentform-clean-emails-log.png
---

If you have **Log Emails** config option in **Payment Form** set to **Yes**, the system will store every emails sent from Payment Form in a database table and make these emails viewable from Payment Form -> Emails Log. This scheduled task is used to deletes emails older than certain Number Days (by default 30 days) from Emails Log to clean up un-necessary data and save hosting space. To use this feature:

## Create and configure the scheduled task

1. Go to **System -> Plugins**, make sure **Task - Payment Form** plugin is enabled.
2. Go to **System -> Scheduled Tasks**, press New button in the toolbar to create a new scheduled task for **Payment Form - Clean Email Logs** task type.
3. Setup all required parameters, save it.

![task-paymentform-clean-emails-log](task-paymentform-clean-emails-log.png "task-paymentform-clean-emails-log")

## Task Basic Fields
This scheduled task should not be run so often. Run it every day should be enough. So you can setup **Basic Fields** to following values

- **Execution Rule**: Set to **Interval, Days**
- **Interval in Days**: Set to the number you want, for example, if you set it to 1, the task will be run every 1 day.
- **Execution Time (UTC)**: Choose the time in the day the task will be executed, for example 10:00 AM.

## Task Parameters
- **Days to delete emails log after it is sent**:  Enter a number here (for example 30) and emails from Emails Log will be deleted after 30 days.