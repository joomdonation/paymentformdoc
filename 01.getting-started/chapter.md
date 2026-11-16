---
title: 'Getting Started'
taxonomy:
    category:
        - docs
---

### Chapter 1

# Getting Started

Learn what Payment Form does, how to install and configure it, and where to get help.

## Quick Start

1. Check the [Requirements](/getting-started/requirements) for your Joomla version and [install Payment Form](/getting-started/installation).
2. Review the currency, sender email, and notification recipients in [General Configuration](/getting-started/configuration/general).
3. [Create a fixed-amount form](/basic-setup/forms/form-types/fixed-amount-payment-form) with fields for the payer's name and email address.
4. Enable [Offline Payment](/basic-setup/payment-plugins/offline-payment) to test the form without charging anyone, or configure your [online payment plugin](/basic-setup/payment-plugins) in test mode if it supports one. Select the payment method in the form's **Advanced Settings**.
5. [Display the form](/frontend-items/display-a-single-form) and submit it from the site frontend. In [Payments Management](/payments-management), check that the amount is correct and that the record shows **Pending** for an offline submission or **Paid** for a successful online test payment. Check that the expected confirmation email arrives.

Before accepting real payments, set the form's payment methods to the ones you plan to offer and switch any online plugins from test to live mode. If you accept offline payments, add your payment instructions to the [offline messages and emails](/getting-started/configuration/messages).
