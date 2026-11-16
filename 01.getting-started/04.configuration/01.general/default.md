---
title: General
media_order: Payment-Form-Configuration.png
---

1. Keep **Load Bootstrap CSS** set to **No** if your site template uses Bootstrap 4, Bootstrap 5, or UIkit 3. You can enable it if your template uses another frontend framework.
2. Use **Css Framework** to select the framework used by your site template. The default is **Bootstrap 5**. If your template uses **Bootstrap 4** or **UIKIT3**, select that option.
3. Set **User Registration Integration** to **Yes** to let customers enter a username and password and create a Joomla account when they use a payment form.
4. Set **Only Create User Account For Success Payment** to **Yes** to delay account creation until the customer completes the payment or an administrator approves it. By default, Payment Form creates the account when the customer submits the form, before processing the payment. If the payment fails or the customer abandons it, the account remains blocked, and the customer cannot use it on a later attempt. We recommend setting this option to **Yes**.
5. Set **Show Login Box** to **Yes** to let existing users log in from the form before paying. We recommend enabling this option if you enable **User Registration Integration**.
6. Set **Enable Captcha** to **Yes** to help prevent spam on your payment forms. Payment Form uses Joomla's CAPTCHA system, so you also need to configure the Joomla reCAPTCHA plugin. See [Joomla's guide to configuring reCAPTCHA](https://docs.joomla.org/How_do_you_use_Recaptcha_in_Joomla%3F).
7. Use **Date Format** to control how Payment Form displays dates. See the [date format characters supported by PHP](https://www.php.net/manual/en/datetime.format.php).
8. Use **Date Custom Field Format** to choose the format for **Date** custom fields on your forms.
9. Use **Currency** to select the currency for payments. If you change it, update **Currency Symbol** as well. The default symbol is `$`.
10. To require customers to accept your terms before paying, create a Joomla article with your terms, select it in **Terms And Conditions Article**, and enable **Show Terms And Conditions Checkbox**. Payment Form displays a checkbox with a link to the article. Customers must select the checkbox to proceed.

![General configuration settings](Payment-Form-Configuration.png "Payment-Form-Configuration")
