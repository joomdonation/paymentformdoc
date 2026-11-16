---
title: Plugins
taxonomy:
    category:
        - docs
published: true
---

# Plugins

Use these plugins to control which payments a form accepts, grant access after payment, or send payment data to another system. Choose the plugin that fits your workflow, then follow its guide to configure the forms that should use it.

| What you want to do | Plugin |
| --- | --- |
| Grant access to restricted Joomla content or update a user's group membership after payment | [Joomla User Groups](/plugins/payment-form-joomla-user-groups) |
| Close a form after it reaches a set number of payments | [Limit Payments](/plugins/payment-form-limit-payments) |
| Require the final amount on a form to fall within a set range | [Validate Payment Amount](/plugins/validate-payment-amount) |
| Send payment data to a CRM or another service over HTTP | [Webhook](/plugins/payment-form-webhook) |
| Run custom PHP code when a payment is saved or succeeds | [PHP Script](/plugins/payment-form-php-script) |
| Synchronize a form's payment records to a tab in Google Sheets | [Google Sheets](/plugins/payment-form-google-sheet) |

The Payment Form package includes the first five plugins. Google Sheets integration is available as a separate paid add-on. Once the plugin is installed, enable it under **System → Plugins**. Reopen the form editor to see the plugin's settings tab.

For other integrations, see [Automatic Form Field Population](/automatic-form-field-population), [Newsletter Integrations](/newsletter-integrations), and [Sell Vouchers & Coupons](/sell-vouchers-and-coupons). To configure a gateway or an offline payment method, see [Payment Plugins](/basic-setup/payment-plugins).
