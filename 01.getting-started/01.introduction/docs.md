---
title: Introduction
taxonomy:
    category:
        - docs
---

## What is Payment Form?

Payment Form is a Joomla extension that lets you create custom forms, collect information, and accept payments on your website. You can use it to collect donations, accept event registrations, or sell products.

## Key Capabilities

- **Flexible payment forms.** Create unlimited forms. Set a fixed amount per form, let customers enter an amount, or calculate the total from their selections, such as ticket type, quantity, and an optional lunch.
- **Custom form layouts.** Place labels beside or above inputs, arrange fields in one to four columns, or build a custom grid with different field widths. Hide labels for individual fields or for the entire form. See [Modern Form Layouts](/basic-setup/forms/modern-form-layouts).
- **22 field types.** Use text inputs, dropdowns, checkboxes, date pickers, file uploads, signatures, and more. Validate entries in the browser and on the server, use input masks for formatted values, and [show or hide fields based on other answers](/basic-setup/custom-fields/field-dependencies).
- **Form prefill and account creation.** Prefill fields using profile data from Joomla, Membership Pro, Community Builder, or JomSocial. You can also let customers create a Joomla account when they submit a payment form.
- **70+ payment options.** Accept payments through PayPal, Authorize.net, eWAY, Stripe, Mollie, Redsys, Square, or an offline method. The package includes several payment plugins, with additional gateways available as paid add-ons. Developers can write their own [payment plugins](/basic-setup/payment-plugins).
- **Tax support.** Set a fixed percentage tax rate for each form or calculate VAT using [EU Tax Rules](/basic-setup/eu-tax-rules).
- **Coupons.** Offer fixed-amount or percentage discounts and limit how many times a coupon can be redeemed.
- **PDF invoices and payment history.** Generate PDF invoices automatically and attach them to customer emails. Signed-in customers can view their payments and download available invoices from their [payment history](/frontend-items/payment-history).
- **Payment notifications and automation.** Send email notifications to customers and administrators. After payment, integrations can assign or remove Joomla user groups, add customers to ACYMailing or Mailchimp, run a custom PHP script, or send payment data to an external URL through a webhook.
- **Payment management.** View, search, edit, and approve payment records in the Joomla administrator area or from the frontend with the appropriate permissions. Export records to Excel or CSV and issue refunds when the payment gateway supports them.
- **Revenue chart.** Track revenue or payment counts over a selected period, filter by form, or compare with the same period last year. Use **Per Form** mode to compare selected forms side by side.
- **Multilingual forms and editable messages.** Translate forms, fields, messages, and emails for multilingual sites. Edit messages and emails in a visual editor and translate language strings in the Joomla administrator area.

## Who Should Use Payment Form?

- **Joomla administrators** who need to set up and manage payments on their sites.
- **Site builders** who build websites that need to accept payments.
- **Organization managers** who need to collect payments, donations, or registrations online.

## What's Included?

- **Main component (`com_pmform`).** Manage Payment Form in the Joomla administrator area and display forms on your site.
- **Two modules.** Display payment forms and form lists in module positions.
- **16 plugins.** Add integrations, automation, and other features.
- **Two libraries.** Provide the MVC framework and payment processing support.

## System Requirements

- **Joomla** 4.4.0 or later, with maintenance-only support for Joomla 3
- **PHP** 7.4.0 or later
- **Web server** running Apache with `mod_rewrite` enabled or Nginx
- **Database** running MySQL 5.6 or later, or MariaDB 10.0 or later

## About This Manual

- Installing, updating, and configuring Payment Form
- Creating and managing forms
- Adding and configuring fields
- Setting up payment gateways
- Configuring taxes and PDF invoices
- Managing payment records
- Setting up coupons and plugin integrations
- Using frontend features and following common workflows

The manual assumes you are familiar with basic Joomla administration, including installing extensions, creating menu items, and managing content.
