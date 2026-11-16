---
title: 'Sell Vouchers & Coupons'
---

Use Payment Form to sell codes that customers can redeem in Events Booking, EShop, or Membership Pro. When a payment succeeds, the integration plugin creates the code in the extension that accepts it. You can email the code to the payer or send it directly to a gift recipient.

| Where customers redeem the code | Setup guide |
| --- | --- |
| During event registration in Events Booking | [Events Booking vouchers](/sell-vouchers-and-coupons/payment-form-events-booking-voucher) |
| At checkout in EShop | [EShop vouchers](/sell-vouchers-and-coupons/payment-form-eshop-voucher) |
| When subscribing to a plan in Membership Pro | [Membership Pro coupons](/sell-vouchers-and-coupons/payment-form-membership-pro-coupon) |

## Set up a form to sell codes

1. Install Payment Form and the extension that will accept the code on the same Joomla site. The three integration plugins are included in the Payment Form package. Enable the one you need under **System → Plugins**.
2. [Create a payment form](/basic-setup/forms/add-new-form) and set the purchase price and payment methods.
3. In the form editor, open the integration's settings tab and enable code generation. It defaults to **No**. Repeat this step for each form that sells codes.
4. Configure the email that should contain the code, then [display the form on your site](/frontend-items/display-a-single-form).

In the integration tab, you can set the code's value independently of the purchase price. For example, charge 50 for a voucher worth 60. Leave the code amount blank to use the payment amount. The plugin uses the gross amount when it is positive and falls back to the recorded total. The resulting code value must be greater than zero.

Set **Number Days** in the plugin to expire codes a set number of days after creation. This setting applies to every form using the plugin. Leave it blank for no expiration.

If you upgraded from a version that used a **Form Ids** list in the plugin, check that generation is enabled in the integration tab on each of those forms.

## Email the code to the payer or a gift recipient

**Email the payer.** For online payments, edit the form and add the integration's code tag to **Messages → User Email Body**. For offline payments, add the tag to **Payment Approved Email Body** under **Payment Form → Configuration → Messages**. The code is generated when you [approve the offline payment](/payments-management/approve-payments).

**Email a gift recipient.** Add a separate [Email custom field](/basic-setup/custom-fields/add-new-custom-field) to the form for the recipient's address. In the integration plugin, select that field and enter the notification subject and body. Include the code tag in the body. The plugin sends this separate message when the field contains a valid email address and both the subject and body are filled in. To address the recipient by name, add a custom field for their name and use its field tag in the message. For delivery only to the recipient, include the code tag only in the plugin's recipient email.

## Test the purchase and redemption

Complete a test payment through the published form. For an offline payment, approve it after submission. Confirm that the code appears in the target extension, that the intended recipient receives it, and that the code works in an eligible registration, order, or subscription.

If the integration tab is missing, check that the plugin is enabled and the target extension is installed. If the payment is marked **Paid** but the email contains no code, check whether the code was created in the target extension. If it was, verify that the email template for that payment type contains the correct tag. If it was not, check that generation is enabled for the form and the code value is greater than zero.

