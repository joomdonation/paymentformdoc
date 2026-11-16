---
title: 'Fixed Amount Payment Form'
published: true
---

Use this setup when everyone pays the same base amount. For example, an **Annual Membership Renewal** form could charge 99 and collect the member's name and email address.

## Setup

1. [Create the form](/basic-setup/forms/add-new-form) and enter `99` in **Amount**.
2. [Assign the contact fields](/basic-setup/forms/customize-form#choose-the-fields-to-display), such as **First Name**, **Last Name**, and **Email**. Use fields with **Fee Field** disabled and leave the built-in **Amount** field unassigned so the payer cannot enter an additional amount.
3. In **Advanced Settings → Payment Methods**, choose how members can pay.
4. [Display the form](/frontend-items/display-a-single-form) and verify the amount with a test payment.

## Result

The base charge is 99 for each renewal. Any configured late fee, coupon discount, tax, or payment-method processing fee still applies.

## When to use fee fields instead

Keep the base amount fixed and add [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) when the form has optional upgrades or add-ons. For example, a 99 membership renewal can include an optional printed certificate for an additional 10.
