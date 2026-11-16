---
title: General
media_order: Payment-Form-Configuration.png
---

The **General** tab controls site-wide defaults for forms, email, formatting, and file uploads.

![General configuration settings](Payment-Form-Configuration.png "Payment-Form-Configuration")

## General Settings

- **Download ID** lets you install Payment Form updates through Joomla's extension updater. Get the ID from your JoomDonation account. See [Installation & Upgrade](/getting-started/installation#update).
- **Css Framework** controls which styles Payment Form uses to match your site template. Choose **Bootstrap 5** (the default), **Bootstrap 4**, or **UIKIT 3**. When **Load Bootstrap CSS** is available, set it to **No** if your template already loads Bootstrap. Set it to **Yes** if you want Payment Form to load Bootstrap's stylesheet.
- **User Registration Integration** lets customers enter a username and password to create a Joomla account when they use a payment form. Individual forms can override this default. Enable **Show Login Box** to let existing users sign in directly from the form.
- **Only Create User Account For Success Payment** delays account creation until payment succeeds or an administrator approves it. With this setting disabled, Payment Form creates the account on submission. A failed or abandoned payment can leave the account blocked and prevent the customer from reusing the same username or email on another attempt.
- **Enable Captcha** uses Joomla's CAPTCHA system to help prevent spam. Enable and configure a compatible CAPTCHA plugin in Joomla before turning on this setting. See also [Anti-Spam Settings](/getting-started/configuration/anti-spam-settings).
- **Show Confirmation Step** lets customers review their details and total before proceeding with the payment. Edit the text above the summary under **Messages → Confirmation Message**.
- **Display Custom Field Description** shows field help as a tooltip, under the field label, or under the input. Choose **Under Field Input** if the instructions should be visible next to the input.
- **Default Country** preselects a country when the form has no country from another source. For EU tax calculations, this setting also identifies the home country. See [EU Tax Rules](/basic-setup/eu-tax-rules).
- **Show Incomplete Payment Records** includes unfinished online payments in the payments list and customer payment history. Pending offline payments appear with either setting so you can approve them when you receive payment.
- **Show Terms And Conditions Checkbox** requires customers to accept your terms. Create a Joomla article with your terms and select it under **Terms And Conditions Article** to link it from the form.

## Mail Settings

- **From Name** and **From Email** set the sender name and address. Leave either field blank to use its value from Joomla's Global Configuration.
- **Reply-To Email** sets the address customers reply to when they respond to Payment Form emails. Notifications to administrators can also include the payer's address for direct replies.
- **Notification Emails** sets the addresses that receive administrator notifications. Separate multiple addresses with commas, for example `payments@example.com,accounting@example.com`. If left blank, Payment Form uses the sender address. Individual forms can specify their own recipients.
- **Use Joomla Mail Template** applies Joomla's global HTML email layout to Payment Form emails. On Joomla 5.2 or later, enable **Mail Template Layout** in Joomla's **Mail Templates** options to make this setting available.

Edit the subjects and bodies under [Messages](/getting-started/configuration/messages).

## Formatting

- **Currency** sets the default currency for payments. **Currency Symbol** and **Currency Position** control how the symbol appears next to the amount. If you change the default currency, update the symbol as well. A form can specify its own currency.
- **Number Of Decimal**, **Decimal Point**, and **Thousands Separator** control how amounts are formatted. For example, use `2` decimal places, a comma for the decimal point, and a period for the thousands separator to display `1.234,56`.
- **Date Format** controls dates shown in Payment Form. **Date Custom Field Format** controls the format for **Date** fields on the form. See [PHP's date format characters](https://www.php.net/manual/en/datetime.format.php) for **Date Format**.
- **CSV Delimiter** lets you choose a comma or semicolon between columns in CSV exports. Choose the delimiter your spreadsheet software expects.

## Privacy Policy (GDPR) Settings

Set **Show Privacy Policy Checkbox** to **Yes** to require customers to accept your privacy policy. Link to a Joomla article with **Privacy Policy Article**, or enter the address of an existing policy page in **Privacy URL**. See [Privacy Policy Checkbox](/basic-setup/gdpr) for details.

## Other Settings

### File uploads

These settings apply when a form includes a **File** custom field.

- **File Upload Path** sets the storage folder relative to your Joomla site root. The default is `images/com_pmform`.
- **Allowed File Types** lists extensions customers can upload. Enter them without leading dots and separate them with commas, for example `pdf,docx`.
- **Upload Max File Size** sets the limit per file in MB. Your server's upload limits also apply.
- **Send Attachment to Admin** adds uploaded files to the administrator's payment notification email.

### Submissions, tracking, and email logs

- **Prevent Double Submissions** helps stop the same form submission from being processed twice, for example when a customer clicks the payment button twice.
- **Tracking Code** inserts your code on Payment Form's built-in completion page for successful payments with a positive total. A form can supply its own tracking code. If you redirect customers to a custom completion URL, add your tracking there.
- **Log Emails** records Payment Form email attempts. Use the [Emails Log](/payments-management/email-log) to check recipients and messages.
