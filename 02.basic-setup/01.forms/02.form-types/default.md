---
title: 'Form Types'
---

Choose an example based on how you want to determine the amount. Each setup uses the same form editor. The form's **Amount** and the [custom fee fields](/basic-setup/custom-fields/custom-fee-fields) assigned to it determine the price.

| What you need | Example | Setup guide |
| --- | --- | --- |
| Collect information without taking a payment | Interest form or free registration | [Information Collection Form](/basic-setup/forms/form-types/information-collection-form) |
| Charge the same base amount to every payer | Annual membership renewal | [Fixed Amount Payment Form](/basic-setup/forms/form-types/fixed-amount-payment-form) |
| Let the payer enter the amount | Donation or invoice payment | [Payer-Entered Amount Form](/basic-setup/forms/form-types/payer-entered-amount-form) |
| Add a price for each selected option | Conference ticket and add-ons | [Option-Priced Payment Form](/basic-setup/forms/form-types/option-priced-payment-form) |
| Calculate prices from quantities or multiple inputs | Training fee per attendee | [Calculated Payment Form](/basic-setup/forms/form-types/calculated-payment-form) |

## How the total is calculated

Payment Form adds the base **Amount** and the fees from custom fields to get the subtotal. For example, a base amount of 100 and a selected add-on priced at 15 give a subtotal of 115.

If configured, Payment Form then adds the late-payment fee, subtracts the coupon discount, adds tax, and adds the payment method's processing fee, in that order.
