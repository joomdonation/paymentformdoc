---
title: 'Information Collection Form'
---

Use this setup for free registrations, enquiries, or surveys. For example, an **Event Interest Form** could ask for the visitor's name, email address, organization, and a comment.

## Setup

1. [Create the form](/basic-setup/forms/add-new-form) and set **Amount** to `0`. Leave **Late Payment Date** blank.
2. [Assign the fields](/basic-setup/forms/customize-form#choose-the-fields-to-display) you want and mark essential fields as required. Use fields with **Fee Field** disabled and leave the built-in **Amount** field unassigned.
3. In **Messages**, set **Thank You Message** to confirm receipt. To notify a different team, enter their addresses under **Advanced Settings → Notification Emails**.
4. Leave **Minimum Payment Amount** blank or set it to `0` under **Configuration → Anti-Spam Settings** so this form can accept a zero total. Use [Validate Payment Amount](/plugins/validate-payment-amount) to set a minimum on individual forms that need one.
5. [Display the form](/frontend-items/display-a-single-form) and test a submission.

## Result

Visitors submit the form directly on your site. Payment Form stores each submission as a zero-amount record in **Payments**, where administrators can review or export it. If **Show Confirmation Step** is enabled, visitors review their details before submitting.
