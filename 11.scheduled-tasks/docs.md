---
title: 'Scheduled Tasks'
taxonomy:
    category:
        - docs
media_order: payments.png
published: true
---

Use the **Task - Payment Form** plugin to run maintenance jobs through Joomla's Scheduled Tasks. You can set up each cleanup task independently.

| Task | When to use it |
| --- | --- |
| [Clean Emails Log](/scheduled-tasks/clean-emails-log) | Keep recent email log entries and remove older ones. |
| [Delete Old PDF Invoices](/scheduled-tasks/delete-old-pdf-invoices) | Free disk space used by generated invoice PDFs. |
| [Delete Incomplete Payments](/scheduled-tasks/delete-incomplete-payments) | Remove pending online payment records from abandoned or failed checkouts. |
| [Delete Old Payments](/scheduled-tasks/delete-old-payments) | Apply a retention period to payment records across all forms and statuses, including paid payments. |

## Create a scheduled task

1. In Joomla's administrator area, go to **System → Plugins** and enable **Task - Payment Form**.
2. Go to **System → Scheduled Tasks**, click **New**, and select the Payment Form task type you want to run.
3. Give the task a **Title**. Under **Basic Fields**, set **Execution Rule** to **Interval, Days**, choose how often it should run in **Interval in Days**, and set **Execution Time (UTC)**.
4. If the task has a **Task Parameters** tab, set the retention period there. Review the settings, set **Status** to **Enabled**, and save the task.

The interval controls how often Joomla runs the task. The retention period controls which entries qualify for deletion on each run. Email and payment record cleanup count calendar days in UTC. Once an entry reaches the configured age, the next run can delete it.

Joomla needs an active scheduler trigger to run due tasks. If a task is overdue, check the scheduler settings under **System → Scheduled Tasks → Options**. If you choose **Test Task → Run Test**, Joomla runs the cleanup immediately and can delete eligible data.
