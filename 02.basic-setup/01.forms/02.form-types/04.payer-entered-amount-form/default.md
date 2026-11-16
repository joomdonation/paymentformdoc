---
title: 'Payer-Entered Amount Form'
published: true
---

Use this form type when the payer chooses the amount to pay. It works well for donations, invoice payments, deposits, and other payments where the administrator does not set one fixed price.

## Example: donation form

The form collects the donor's name, email address, and donation amount. If the donor enters 25, the payment total is 25 before any configured tax or payment-method fee.

## Setup with the built-in Amount field

1. Create a form named **Make a Donation**.
2. Set the form's **Amount** to `0` or leave it empty.
3. Assign the built-in **Amount** field to this form.
4. Edit the **Amount** field and confirm that **Fee Field** is **Yes** and **Fee Formula** is `[FIELD_VALUE]`.
5. Make the field required if a payer must enter an amount.
6. Select the payment methods in the form's **Advanced Settings**.
7. Test the form with several amounts before publishing it.

## Use a separate amount field

You can create a dedicated **Number** field instead of using the built-in **Amount** field. For example, create a field named `donation_amount`, set **Fee Field** to **Yes**, and use this formula:

```text
[FIELD_VALUE]
```

Use a **Number** field when possible, and set a minimum value if the payment must meet a minimum amount.

## Result

The field value becomes a custom fee. Since the base form amount is zero, the fee is the payment total. You can still add a fixed base amount or additional fee fields if the payment flow requires them.

For formula behavior and numeric input rules, see [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields).