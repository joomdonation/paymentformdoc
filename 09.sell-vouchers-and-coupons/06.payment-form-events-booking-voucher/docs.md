---
title: 'Events Booking Voucher'
taxonomy:
    category:
        - docs
---

Sell codes that customers can enter in the coupon field when registering for an event. Each successful payment on a configured form creates a code in Events Booking.

## Enable the plugin and configure the form

1. In Joomla, go to **System → Plugins** and enable **Payment Form - Events Booking Voucher**. To set an expiration period for this integration, enter the number of days in **Number Days**. Leave it blank for no expiration.
2. Go to **Components → Payment Form → Forms**, open the form that sells the vouchers, and select **EB Voucher Settings**.
3. Set **Enable Events Booking Voucher Generation** to **Yes**, configure the options below, and save the form.

| Setting | What to choose |
| --- | --- |
| **Coupon Type** | Choose **Voucher** to let customers use the remaining balance on later eligible registrations. This is the default. Choose **Fixed Amount** to give a set discount per use. |
| **Voucher Amount** | Enter a positive whole number to set the face value, or leave it blank to use the payment amount. |
| **Voucher Times** | Set the maximum number of uses per code. Leave it blank or enter `0` for no usage count limit. A **Voucher** can be used while it still has a balance. |
| **Categories** | Select the Events Booking categories where the code can be redeemed. Leave all categories unselected to allow redemption in any category. |

## Email the code

Use the tags below in the payer's payment email or in the plugin's gift notification. For gift delivery, select the recipient's custom field in **Voucher Receive Email Field** and fill in **Voucher Notification Email Subject** and **Voucher Notification Email Body**. See [how to configure delivery to the payer or a gift recipient](/sell-vouchers-and-coupons#email-the-code-to-the-payer-or-a-gift-recipient).

| Tag | Inserts |
| --- | --- |
| `[VOUCHER_CODE]` | The code to enter when registering. |
| `[VOUCHER_AMOUNT]` | The initial value of the voucher or the fixed discount amount. |
| `[VOUCHER_VALID_TO]` | The expiration date when **Number Days** is set. |
| `[VOUCHER_TIMES]` | The maximum number of uses when **Voucher Times** is greater than zero. |
