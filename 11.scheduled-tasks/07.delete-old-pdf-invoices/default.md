---
title: 'Delete Old PDF Invoices'
media_order: task-paymentform-delete-old-pdf-invoices.png
published: true
---

Use this task if your site generates PDF invoices and you want to reclaim disk space. On each run, it deletes PDF files in `media/com_pmform/invoices` that were last modified more than 24 hours ago.

Payment Form generates a fresh PDF from the payment record when someone downloads the invoice from the administrator payments list or from **Payment History**. See [Invoice Settings](/getting-started/configuration/invoice-settings).

## Configure the task

1. [Create a scheduled task](/scheduled-tasks#create-a-scheduled-task) of type **Payment Form - Delete Old Invoices**.
2. Under **Basic Fields**, set **Interval in Days** to **7** for weekly cleanup, or choose a shorter interval if your site generates many invoices.

The 24-hour cutoff is fixed. Only the schedule is configurable.

![Joomla settings for the Delete Old Invoices task](task-paymentform-delete-old-pdf-invoices.png)
