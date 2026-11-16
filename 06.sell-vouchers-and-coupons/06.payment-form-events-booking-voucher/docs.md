---
title: 'Events Booking Voucher'
taxonomy:
    category:
        - docs
---

This plugin gives you a way to sell voucher for Events Booking extension. You can configure it so that each time someone makes payment using the configured forms, the plugin will generate voucher code with the payment amount in Events Booking. The voucher code will be sent to user (or any user the payer want) and then the user can use that voucher code to receive discount while registering for events in Events Booking.

## Enable And Configure Plugin

To use this feature, please find and enable **Payment Form - Events Booking Voucher** plugin. The plugin has the following parameters :

- **Form Ids**: Enter IDs of the forms which you want to generate voucher codes when someone makes payment using that form (comma separated). You must enter IDs of the forms you want here, otherwise, no voucher will be generated.
- **Number Days**: If you want the voucher to be valid for only certain number of days since the time it is created, enter the number into this parameter. Leave it empty and there will be no time limit for using the voucher.

### Advanced Parameters
If you want to send the received voucher code to a different user (not the user who is making the payment), please create a custom field to allow entering email of that receiver in the form. Then configure the parameters below in the plugin:

- **Voucher Receive Email Field** : Select the the field you created above
- **Voucher Notification Email Subject** : Enter subject of the email which will be sent to the the user who receives the voucher.
- **Voucher Notification Email Body** : Enter the email message which will be sent to the user who receives the voucher

For the email, you can use any tags like the in the email sent from payment form extension. The most important tags (related to voucher data are): [VOUCHER_CODE], [VOUCHER_AMOUNT], [VOUCHER_VALID_TO] , [VOUCHER_TIMES] 

### Send Voucher Code

In case you do not use advanced parameters above, you can still edit the email message of your form, insert the tags above (beside normal tags) to send voucher code to the user who makes payment [VOUCHER_CODE], [VOUCHER_AMOUNT], [VOUCHER_VALID_TO] , [VOUCHER_TIMES] 

### Use Fixed Voucher Amount

If you want to create voucher with fixed payment amount (instead of the amount users make payment on the form), edit the form, look at Voucher Settings tab, enter the voucher amount there. Then all vouchers created for that form will have that fixed amount, not depend on how much users pay.