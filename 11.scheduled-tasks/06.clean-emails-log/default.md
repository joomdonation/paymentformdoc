---
title: 'Clean Emails Log'
media_order: task-paymentform-clean-emails-log.png
---

Use this task to limit how long Payment Form keeps entries in **Payment Form → Emails Log**. It's useful when **Log Emails** is enabled and you want to keep recent entries for troubleshooting. See [General configuration](/getting-started/configuration/general).

## Configure the task

1. [Create a scheduled task](/scheduled-tasks#create-a-scheduled-task) of type **Payment Form - Clean Email Logs**.
2. Under **Basic Fields**, set **Interval in Days** to **1** to clean the log daily.
3. Under **Task Parameters**, set **Days to delete emails log after**. The default is **30 days** and the minimum is **1 day**. On each run, the task deletes log entries sent at least that many days ago.

![Joomla settings for the Clean Email Logs task](task-paymentform-clean-emails-log.png)
