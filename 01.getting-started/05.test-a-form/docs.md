---
title: 'Test a Form'
taxonomy:
    category:
        - docs
---

Test the published form from the page your customers will use. Use a guest session or an account with the same Joomla access as your intended audience. If you take online payments, use a test site and your gateway's sandbox or test mode when available.

## Submit the form

1. Confirm the right fields appear. Try required fields, conditional questions, and any file uploads.
2. Check the total after selecting priced options, entering an amount, or applying a coupon. Confirm the currency and any tax or processing fee.
3. Submit the form and review the confirmation, payment instructions, and any emails you configured. Open **Components → Payment Form → Payments** and find the record.

| Form or payment method | What to verify |
| --- | --- |
| Information collection or a zero total | The form submits without asking for payment. The record appears as **Paid** with a zero amount. |
| Offline payment | The customer sees instructions for paying manually and the record is **Pending**. For a test record, follow [Approve Payments](/payments-management/approve-payments) to verify the status change and any configured approval email or integration. |
| Online payment | Complete the checkout with the gateway's test credentials or test payment details. Confirm that both the gateway and Payment Form show the payment succeeded and that the amount matches. |

If you offer invoices, verify that you can open the PDF and that it reaches the customer through the channels you enabled. For [Payment History](/frontend-items/payment-history), make the test payment while signed in and check the invoice download with the same account. Test any form-specific integration, such as a mailing list subscription, after the payment reaches **Paid**.

## Troubleshoot the result

| What you see | What to check |
| --- | --- |
| The form is missing or inaccessible | Check the form's **Published**, **Publish Up**, **Publish Down**, and **Access** settings. Then check the [menu item, module, or article](/frontend-items) displaying it. |
| A payment method is missing | Make sure the total is greater than zero and the payment plugin is published. Check the plugin's **Access** and the form's **Advanced Settings → Payment Methods**. [Payment Plugins](/basic-setup/payment-plugins#configure-and-test-a-payment-method) |
| The gateway shows a successful payment, but the record is pending or missing | Look for the record with **Show Incomplete Payment Records** enabled in [General Configuration](/getting-started/configuration/general#general-settings). Check the plugin's test or live credentials and the gateway's notification or webhook settings against its setup guide. |
| The expected email is missing | Check the payment status and the [Emails Log](/payments-management/email-log). |
| The expected invoice is missing | Check [Invoice Settings](/getting-started/configuration/invoice-settings), including whether invoices for offline payments are deferred until approval. |

## Switch an online payment method to live mode

Set the form's **Payment Methods** to the methods you intend to offer. In each online payment plugin, switch to live mode and enter the live credentials. If the gateway uses webhooks, configure the live endpoint and its signing credentials using the gateway's setup guide. Open the live form as a customer to verify the payment methods, currency, and total.
