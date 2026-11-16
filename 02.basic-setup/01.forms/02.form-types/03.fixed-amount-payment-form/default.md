---
title: 'Fixed Amount Payment Form'
published: true
---

Use this form type when every payer owes the same amount. The administrator sets the amount on the form, and the payer supplies only the information needed to complete the payment.

## Example: annual membership renewal

Every member pays 99 for renewal. The form collects the member's name and email, then sends them to a selected payment method to pay 99.

## Setup

1. Create a form named **Annual Membership Renewal**.
2. Enter `99` in the form's **Amount** setting.
3. Do not assign the built-in **Amount** field to this form. This prevents the payer from changing the fixed amount.
4. Do not enable **Fee Field** on the form's custom fields.
5. Assign the contact fields you need, such as **First Name**, **Last Name**, and **Email**.
6. In **Advanced Settings**, choose the payment methods available for this form.
7. Publish the form and make a test payment.

## Result

The payment total is always 99 before any configured late fee, coupon discount, tax, or payment-method processing fee. The payer cannot change the base amount.

## When to use fee fields instead

Keep the base amount fixed and add [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) when the form has optional upgrades or add-ons. For example, a 99 membership renewal can include an optional printed certificate for an additional 10.