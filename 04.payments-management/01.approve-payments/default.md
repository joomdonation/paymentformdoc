---
title: 'Approve Payments'
---

Payment Form records offline payments, such as bank transfers, as **Pending** while you wait for the money to arrive. Mark the payment as **Paid** once you receive it.

## Mark an offline payment as paid

1. Open **Components → Payment Form → Payments**.
2. Find the pending record and check the payer, payment method, and amount against the payment you received.
3. Select the record's checkbox and click **Publish**. You can select several records after verifying receipt for each one. To approve a record while editing it, set **Paid** to **Yes** and save.

Payment Form changes the status to **Paid** and runs any payment-success integrations configured for the form. It also sends the approval email if the customer has a valid email address and the approval email subject is set.

To edit the approval message, go to **Payment Form → Configuration → Messages** and update **Payment Approved Email Subject** and **Payment Approved Email Body**. See [Messages](/getting-started/configuration/messages).

If you approved an offline payment by mistake, select the record and click **Unpublish** to return it to **Pending**. Approving it again can run the configured payment-success integrations a second time.
