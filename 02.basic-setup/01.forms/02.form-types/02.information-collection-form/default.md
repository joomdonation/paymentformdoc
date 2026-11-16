---
title: 'Information Collection Form'
---

Use this form type to collect registrations, requests, surveys, or other information without charging the payer. When the final amount is zero and the form has no fee fields, Payment Form submits the record without displaying payment methods.

## Example: event interest form

Create a form named **Event Interest Form** and add fields such as **First Name**, **Last Name**, **Email**, **Organization**, and **Comment**. The payer can submit their information, and administrators can review or export the resulting records.

## Setup

1. Create a form and set **Amount** to `0` or leave it empty.
2. Do not assign the built-in **Amount** field to the form.
3. Do not enable **Fee Field** on any custom field assigned to the form.
4. Assign the information fields you need and mark essential fields as required.
5. Set the form's notification emails if submissions should be sent to a different team.
6. Publish the form.

## Result

The form displays a **Submit** button. It stores the submitted information as a payment record with a zero amount, but does not ask the user to select a payment method or visit a payment gateway.

## Useful additions

- Use [Field Dependencies](/basic-setup/custom-fields/field-dependencies) to display follow-up questions only for relevant selections.
- Use the **Messages** tab on the form to provide a submission confirmation specific to this form.
- Restrict the form with **Access** when it is intended for registered users or a specific Joomla user group.