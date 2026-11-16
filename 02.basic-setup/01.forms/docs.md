---
title: Forms
taxonomy:
    category:
        - docs
process:
    markdown: true
    twig: true
media_order: forms.png
---

Use Payment Form to collect anything from a fixed invoice payment to a donation where the payer enters the amount. You can also collect information without taking a payment.

## Set up a form

1. [Choose how to determine the amount](/basic-setup/forms/form-types). Each example shows which form settings and fields to use.
2. [Create the form](/basic-setup/forms/add-new-form). Set the base amount, access level, and payment methods for this form.
3. [Configure the fields and checkout experience](/basic-setup/forms/customize-form). Decide what to collect, whether to offer login and registration, and what to show after submission.
4. [Choose a layout](/basic-setup/forms/modern-form-layouts). Set the number of columns, field widths, and label placement.
5. [Display the form on your site](/frontend-items/display-a-single-form) and [test the full submission](/getting-started/test-a-form), including the payment status and emails.

## Manage existing forms

In the Joomla administrator area, go to **Components → Payment Form → Forms**. You can also select **Forms** from the Payment Form dashboard or open **Setup → Forms** from another Payment Form page.

![Forms list showing titles, publish dates, payment counts, paid amounts, and IDs](forms.png)

- Select a form's title to edit it, or select **New** to create one.
- Use the **Published** column to open or close a form. Set **Publish Up** and **Publish Down** in the editor if it should open or close on specified dates.
- Open an existing form and select **Save as Copy** to reuse its settings and any custom fields assigned specifically to it. Review the copy's title, amount, payment methods, and fields. If you excluded the original form from a shared field, update that field's exclusions to include the copy where needed.
- The payment count and **Paid Amount** columns summarize records marked **Paid**, including zero-amount submissions. Select the count to open the **Payments** list filtered to that form.
- Use the form's **ID** when embedding it in an article.
