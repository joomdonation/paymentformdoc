---
title: 'Payment History'
taxonomy:
    category:
        - docs
---

Add **Payment History** to your site so customers can review their payment records and download available PDF invoices after signing in to Joomla.

## Create a Payment History page

1. In the Joomla administrator area, open **Menus**, select the site menu where the link should appear, and click **New**.
2. Enter a **Menu Title**, such as **My Payments**. Under **Menu Item Type**, click **Select** and choose **Payment Form → Payment History**.
3. Set **Access** to **Registered** to make the link available to signed-in users. If you want guests to see the link, use **Public**. Payment History sends guests who follow a public link to the Joomla login page.
4. Set **Status** to **Published** and save. Open the page with a customer account that has made a payment to confirm that the record appears.

The page shows the form title, payment date, amount, and transaction ID. Published fields with **Show On Payments List** enabled appear as additional columns.

## Let customers download invoices

1. In **Components → Payment Form → Configuration → Invoice Settings**, set **Activate Invoice Feature** to **Yes**. See [Invoice Settings](/getting-started/configuration/invoice-settings) for when invoices are issued, including for pending offline payments.
2. Make a test payment while signed in with a customer account. Open **Payment History** with that account and click the invoice number in the **Invoice Number** column to download the PDF.

Payment History can show a payment when its email address matches the signed-in user's account. The invoice download requires the payment record to be linked to that Joomla account. If customers need to download their invoices from this page, ask them to sign in before paying, or set the payment form's **Access** to **Registered** to require it. See [Registration and login](/basic-setup/forms/customize-form#registration-and-login) for form setup options.
