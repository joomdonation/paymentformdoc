---
title: 'EShop Voucher'
taxonomy:
    category:
        - docs
---

Sell gift vouchers that customers can redeem at checkout in EShop. Each successful payment on a configured form creates a voucher in EShop.

## Enable the plugin and configure the form

1. In Joomla, go to **System → Plugins** and enable **Payment Form - EShop Voucher**. To set an expiration period for this integration, enter the number of days in **Number Days**. Leave it blank for no expiration.
2. Go to **Components → Payment Form → Forms**, open the form that sells the vouchers, and select **Eshop Voucher Settings**.
3. Set **Enable EShop Voucher Generation** to **Yes**. In **Voucher Amount**, enter a positive whole number to set the voucher's face value, or leave it blank to use the payment amount. Save the form.

## Email the voucher code

Use the tags below in the payer's payment email or in the plugin's gift notification. For gift delivery, select the recipient's custom field in **Voucher Receive Email Field** and fill in **Voucher Notification Email Subject** and **Voucher Notification Email Body**. See [how to configure delivery to the payer or a gift recipient](/sell-vouchers-and-coupons#email-the-code-to-the-payer-or-a-gift-recipient).

| Tag | Inserts |
| --- | --- |
| `[ESHOP_VOUCHER_CODE]` | The code to enter at checkout. |
| `[ESHOP_VOUCHER_AMOUNT]` | The voucher's value. |
| `[ESHOP_VOUCHER_VALID_TO]` | The expiration date when **Number Days** is set. |
