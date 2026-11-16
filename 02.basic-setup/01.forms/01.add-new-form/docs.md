---
title: 'Add New Form'
taxonomy:
    category:
        - docs
published: true
media_order: Payment-Form-Form-General-Settings.png
---

Go to **Components → Payment Form → Forms** and select **New**. Configure the form, then set up its custom fields, payment methods, and messages as needed. The editor has **General**, **Messages**, **Advanced Settings**, and **Custom JavaScript** tabs. Additional tabs can appear when multilingual support or installed integrations provide them.

![Form general settings](Payment-Form-Form-General-Settings.png "Form general settings")

## General

| Setting | Description |
| --- | --- |
| **Title** | The form name shown to payers. Use a specific title, such as `Conference registration` or `Annual membership renewal`. |
| **Amount** | The form's base amount. Leave it blank or enter `0` to let payers enter an amount through an **Amount** custom field. For a fixed-price form, enter the amount here and do not assign the **Amount** custom field to this form. Custom fee fields can add to the base amount. |
| **Tax Rate** | The percentage tax rate for this form. This setting is shown only when EU VAT Rules are not enabled. |
| **Publish Up** | The date and time from which the form accepts payments. Leave blank to make it available immediately when published. |
| **Publish Down** | The date and time after which the form stops accepting payments. Leave blank for no closing date. |
| **Late Payment Fee** | An extra charge for payments made after **Late Payment Date**. Enter an amount and select either **Percent** or **Fixed Amount**. The percentage is calculated from the form total after custom field fees. |
| **Late Payment Date** | The date after which the late-payment fee applies. Leave blank to disable the late fee. |
| **PayPal Account** | A PayPal account or email address to use for this form. Leave blank to use the account configured in the PayPal payment plugin. |
| **Form Layout** | Select a built-in layout: **Default**, **Modern**, **Inline**, **2 Columns 2 Lines**, or **2 Columns Inline**. Installed layouts can also appear in this list. |
| **Number Columns** | Available with the **Modern** layout. Select 2, 3, or 4 to give every normal-position field the same column width. Select the default value to use each field's own **Container Size**. |
| **Form Format** | Available with the **Modern** layout. **Horizontal** places labels beside controls where the site framework supports it; **Stacked** places labels above controls. |
| **Show Fields Label** | Choose **Use Field Setting** to keep each field's own label setting, or choose **Yes** or **No** to override it for every field on this form. |
| **Access** | The Joomla access level required to view and use the form. |
| **Custom Payment Complete URL** | Redirects the payer to this URL after payment is completed. Leave blank to display the normal Payment Form completion page. |
| **Terms And Conditions Article** | Select a Joomla article to show as this form's terms and conditions. Leave blank to use the article configured globally, if any. |
| **Attachment** | A file sent to the payer with the payment email. Upload or copy the file to `media/com_pmform` first, then select it here. The selectable file types follow the component's allowed-extensions configuration. |
| **Enable Coupon** | Shows the coupon-code input for this form. Enable it only when payers should be able to redeem coupons. |
| **Published** | A form must be published and within its publish dates to accept payments. |

## Messages

Use this tab to override the messages and email templates configured globally. Leave a message or template empty to use the corresponding configuration value.

| Setting | Description |
| --- | --- |
| **Form Message** | Displays above the payment form. You can use `[FORM_TITLE]` and `[AMOUNT]`. |
| **Confirmation Message** | Displays above the confirmation step when confirmation is enabled. You can use `[FORM_TITLE]` and `[AMOUNT]`. |
| **Thank You Message** | Displays after a successful online payment. |
| **Thank You Message (Offline Payment)** | Displays after an offline payment is submitted. |
| **Cancel Message** | Displays when the payer cancels a payment. |
| **Admin Email Subject** | The subject of the notification sent to the form's notification email addresses. |
| **Admin Email Body** | The body of the payment notification sent to administrators. |
| **User Email Subject** | The subject of the payment email sent to the payer. |
| **User Email Body** | The body of the payment email sent to the payer after an online payment. |
| **User Email Body (Offline Payment)** | The body of the payment email sent to the payer after an offline payment. |

Email and message templates support replacement tags. Use the same tag format as the global templates, for example `[FORM_TITLE]`, `[AMOUNT]`, and `[PAYMENT_DETAIL]`.

## Advanced Settings

| Setting | Description |
| --- | --- |
| **Notification Emails** | Comma-separated addresses that receive payment notifications for this form. Leave blank to use the global notification addresses. |
| **Payment Methods** | Restrict the form to selected published payment methods. Choose **All Payment Methods** to use every published method. |
| **Currency** | The currency used for payments from this form. Select **Default** to use the component's global currency. |
| **Currency Symbol** | Overrides the currency symbol displayed for this form. Leave blank to use the global symbol. |
| **User Registration Integration** | Controls whether payers can create a Joomla account while submitting this form. Choose **Use Global** to inherit the component setting. |
| **Show Login Box** | Controls whether a visitor is shown the login and account-creation flow for this form. Choose **Use Global** to inherit the component setting. |
| **Invoice Format** | Overrides the global invoice template for payments from this form. Leave blank to use the global invoice format. This setting has an effect when invoices are enabled in the component configuration. |

Some installations also show payment-provider credentials in this tab, such as Authorize.net or PayPal Standard Checkout credentials. These fields are available only when the relevant provider integration adds them.

## Custom JavaScript

The **Custom JavaScript Code** tab adds JavaScript to this form's front-end page. Use it only for form-specific behavior that cannot be configured through Payment Form settings, and test it on a non-production form before publishing.

## Translation and integration settings

When Joomla multilingual support is enabled, the **Translation** tab lets you translate the form title, messages, email subjects, and email bodies for each configured language.

Payment Form plugins and custom integrations can add their own tabs to the form editor. Their fields are specific to the installed integration.