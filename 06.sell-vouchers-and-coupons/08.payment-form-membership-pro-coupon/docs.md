---
title: 'Membership Pro Coupon'
taxonomy:
    category:
        - docs
published: true
---

Sell fixed-amount coupons that customers can redeem on eligible Membership Pro plans. Each successful payment on a configured form creates a coupon in Membership Pro. For a recurring subscription, the discount applies to the first payment only.

## Enable the plugin and configure the form

1. In Joomla, go to **System → Plugins** and enable **Payment Form - Membership Pro Coupon**. To set an expiration period for this integration, enter the number of days in **Number Days**. Leave it blank for no expiration.
2. Go to **Components → Payment Form → Forms**, open the form that sells the coupons, and select **MP Coupon Settings**.
3. Set **Enable Membership Pro Coupon Generation** to **Yes**, configure the options below, and save the form.

| Setting | What to choose |
| --- | --- |
| **Coupon Amount** | Enter a positive whole number to set the discount, or leave it blank to use the payment amount. |
| **Times** | Set the maximum number of uses per coupon. The default is `1`. Enter `0` to allow unlimited uses. |
| **Plans** | Select the Membership Pro plans that accept the coupon. Leave all plans unselected to allow redemption on any plan. |
| **Assign Coupon To User** | Set to **Yes** to restrict redemption to the payer's Joomla account. Use this option with a form that requires a Joomla account. For gifts, leave it set to **No** so the recipient can redeem the coupon. |

## Email the coupon code

Use the tags below in the payer's payment email or in the plugin's gift notification. For gift delivery, select the recipient's custom field in **Coupon Receive Email Field** and fill in **Coupon Notification Email Subject** and **Coupon Notification Email Body**. See [how to configure delivery to the payer or a gift recipient](/sell-vouchers-and-coupons#email-the-code-to-the-payer-or-a-gift-recipient).

| Tag | Inserts |
| --- | --- |
| `[MP_COUPON_CODE]` | The code to enter when subscribing. |
| `[MP_COUPON_AMOUNT]` | The fixed discount amount. |
| `[MP_COUPON_VALID_TO]` | The expiration date when **Number Days** is set. |
