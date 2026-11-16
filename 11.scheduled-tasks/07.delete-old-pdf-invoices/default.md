---
title: 'Delete Old PDF Invoices'
media_order: task-paymentform-delete-old-pdf-invoices.png
published: true
---

Each time Payment Form generates PDF invoice, a PDF file for that invoice will be generated and stored on server and costs hosting space. This scheduled task is used to delete invoice PDFs which are older than one day each time it is executed. To use this feature:

## Create and configure the scheduled task

1. Go to **System -> Plugins**, make sure **Task - Payment Form** plugin is enabled.
2. Go to **System -> Scheduled Tasks**, press New button in the toolbar to create a new scheduled task for **Payment Form - Delete Old Invoices** task type.
3. Setup all required parameters, save it.

![task-paymentform-delete-old-pdf-invoices](task-paymentform-delete-old-pdf-invoices.png "task-paymentform-delete-old-pdf-invoices")

## Task Basic Fields
This scheduled task should not be run so often. Run it every few days should be enough. So you can setup **Basic Fields** to following values

- **Execution Rule**: Set to **Interval, Days**
- **Interval in Days**: Set to the number you want, for example, if you set it to 7, the task will be run every 7 days.
- **Execution Time (UTC)**: Choose the time in the day the task will be executed, for example 10:00 AM.