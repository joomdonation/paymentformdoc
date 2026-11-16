---
title: 'Payer-Entered Amount Form'
published: true
---

Use this setup for donations, deposits, or invoice payments where the payer enters the amount. In the example below, a donor who enters 25 pays a base total of 25 before any configured adjustments.

## Setup with the built-in Amount field

1. [Create a form](/basic-setup/forms/add-new-form) named **Make a Donation** and set its **Amount** to `0`.
2. In **Custom Fields**, open the built-in **Amount** field. Check that it is published and [assigned to the form](/basic-setup/forms/customize-form#choose-the-fields-to-display).
3. Confirm that **Fee Field** is **Yes** and **Fee Formula** is `[FIELD_VALUE]`. Set **Required** to **Yes** if the payer must enter an amount.
4. Assign the donor's name and email fields, then select the payment methods under **Advanced Settings → Payment Methods** in the form editor.
5. [Display the form](/frontend-items/display-a-single-form) and test with several amounts, including a decimal amount if you accept one.

## Use a separate amount field

To give this form its own label or input limits, create a **Number** field titled **Donation Amount** with the name `donation_amount`. Assign it to this form, set **Fee Field** to **Yes**, and enter `[FIELD_VALUE]` in **Fee Formula**. Use **Min**, **Max**, and **Step** to control the input. For example, set **Step** to `0.01` to allow amounts in cents. Use one amount field on the form so the entered amount is added once.

To require a positive payment or enforce a minimum on the final total for this form, use the [Validate Payment Amount](/plugins/validate-payment-amount) plugin. A required field can still have a value of `0`.

## Result

The amount field adds the value the payer enters. With a base amount of `0` and no other fees, this value is the form subtotal.

For formula behavior and numeric input rules, see [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields).
