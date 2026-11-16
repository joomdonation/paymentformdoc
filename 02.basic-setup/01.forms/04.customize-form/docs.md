---
title: 'Customize a Form'
taxonomy:
    category:
        - docs
---

## Choose the fields to display

In Joomla, go to **Components → Payment Form → Custom Fields**. Start with the built-in fields, such as **First Name**, **Last Name**, and **Email**, and add the fields this form needs. For an invoice payment, for example, add a required **Invoice Number** field and assign it only to that form.

| To use a field on | Set **Field Assignment** to |
| --- | --- |
| Every form | **All Forms** |
| Specific forms | **All Selected Forms**, then select those forms under **Forms** |
| Every form except a few | **All Except Selected Forms**, then select the forms to exclude |

Set **Published** to **Yes** for fields that should appear. Set **Required** to **Yes** for fields the payer must complete. To remove a shared field from one form, change its assignment. The field's published status, validation, label, and width settings are shared across the forms that use it.

Set the order in the **Custom Fields** list. Within each section of the form, fields appear in that order. See [Add New Custom Field](/basic-setup/custom-fields/add-new-custom-field) for field settings and [Modern Form Layouts](/basic-setup/forms/modern-form-layouts) for columns, labels, and field placement.

Use [Field Dependencies](/basic-setup/custom-fields/field-dependencies) to ask follow-up questions only when a payer selects a relevant option. For example, show a **Company Name** field when the payer selects **Business** as the customer type.

## Registration and login

Set the site-wide defaults in **Components → Payment Form → Configuration**. To change them for one form, open that form's **Advanced Settings** tab. Each setting offers **Use Global**.

| What you want | Form settings |
| --- | --- |
| Let guests submit without creating an account | Set **Access** to **Public** on **General** and **User Registration Integration** to **No**. |
| Let new users create an account and existing users sign in from the form | Set **Access** to **Public** and set both **User Registration Integration** and **Show Login Box** to **Yes**. Guests see the account fields as part of the form. |
| Require an existing Joomla account before users reach the form | Set **Access** to **Registered** or another appropriate Joomla viewing access level. |

When **User Registration Integration** is enabled, guests enter a username and password even if **Show Login Box** is disabled. Payments submitted while signed in are associated with the user's Joomla account. To prefill fields for returning users, see [Automatic Form Field Population](/automatic-form-field-population).

## Customize the confirmation

Use the form's **Messages** tab to tell payers what to expect and what to do after submitting. For an offline payment, include payment instructions in both **Thank You Message (Offline Payment)** and **User Email Body (Offline Payment)**. Keep the built-in completion page to display the thank-you message, or put those instructions on your own page and enter its URL under **Custom Payment Complete URL**.

To let payers review their details before submitting, enable **Show Confirmation Step** in [Configuration](/getting-started/configuration/general#general-settings), then edit the form's **Confirmation Message** as needed.

## Test the form on your site

Set the form's **Published** setting to **Yes** and make sure its **Publish Up** and **Publish Down** dates allow access. After you [display the form](/frontend-items/display-a-single-form), open the same page your payers will use. Check the layout on desktop and mobile, try any conditional fields, and verify the total and available payment methods. Submit the form and check the resulting record in **Payments**, the confirmation page, and any emails you configured. If the form uses Joomla access levels, repeat the test as a guest or a user with the intended access.
