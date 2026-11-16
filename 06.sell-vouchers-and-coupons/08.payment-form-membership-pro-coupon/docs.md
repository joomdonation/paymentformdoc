---
title: 'Membership Pro Coupon'
taxonomy:
    category:
        - docs
published: true
---

This plugin gives you a way to sell coupon for Membership Pro extension. You can configure it so that each time someone makes payment using the configured forms, the plugin will generate coupon code with the payment amount in Membership Pro. The coupon code will be sent to user (or any user the payer want) and then the user can use that coupon code to receive discount while registering for events in Membership Pro.

## Enable And Configure Plugin

To use this feature, please find and enable **Payment Form - Membership Pro Coupon** plugin. The plugin has the following parameters:

- **Form Ids**: Enter IDs of the forms which you want to generate coupon codes when someone makes payment using that form (comma separated). You must enter IDs of the forms you want here, otherwise, no coupon will be generated.
- **Number Days**: If you want the coupon to be valid for only certain number of days since the time it is created, enter the number into this parameter. Leave it empty and there will be no time limit for using the coupon

### Advanced Parameters
If you want to send the generated coupon code to a different user (not the user who is making the payment), please create a custom field to allow entering email of that receiver in the form. Then configure the parameters below in the plugin:

- **Coupon Receive Email Field** : Select the the field you created above
- **Coupon Notification Email Subject** : Enter subject of the email which will be sent to the the user who receives the coupon.
- **Coupon Notification Email Body** : Enter the email message which will be sent to the user who receives the coupon

For the email, you can use any tags like the in the email sent from payment form extension. The most important tags (related to voucher data are): [MP_COUPON_CODE], [MP_COUPON_AMOUNT], [MP_COUPON_VALID_TO]

### Send Voucher Code

In case you do not use advanced parameters above, you can still edit the email message of your form, insert the tags above (beside normal tags) to send voucher code to the user who makes payment [MP_COUPON_CODE], [MP_COUPON_AMOUNT], [MP_COUPON_VALID_TO]

### Use Fixed Coupon Amount

If you want to create coupon with fixed payment amount (instead of the amount users make payment on the form), edit the form, look at **MP Coupon Settings** tab, enter the amount there. Then all coupons created for that form will have that fixed amount, not depend on how much users pay.