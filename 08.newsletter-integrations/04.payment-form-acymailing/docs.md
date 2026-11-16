---
title: AcyMailing
taxonomy:
    category:
        - docs
published: true
media_order: acymailing.png
---

Use **Payment Form - AcyMailing** to subscribe customers to AcyMailing lists after a successful payment. The plugin looks up the contact by the email address on the payment. It uses the existing contact when it finds one or creates a contact using the payer's email and name.

## Enable the plugin and choose mailing lists

1. Install and enable AcyMailing on the same Joomla site as Payment Form. Create the mailing lists you want to use in AcyMailing.
2. In the Joomla administrator area, go to **System → Plugins** and enable **Payment Form - AcyMailing**.
3. Go to **Components → Payment Form → Forms**, open the form, and select the **AcyMailing Settings** tab.
4. In **Assign To Mailing Lists**, select one or more lists and save the form. Repeat this step for each form you want to connect to AcyMailing.

![AcyMailing Settings tab with a mailing list selected](acymailing.png)

## Test the integration

Complete a test payment through the form, then look up the email address in AcyMailing and check that the contact is subscribed to the selected lists. If you use an offline payment method, [approve the payment](/payments-management/approve-payments) before checking the subscription.

If the **AcyMailing Settings** tab is missing, check that both AcyMailing and the Payment Form plugin are enabled. If the contact is missing after the payment is marked **Paid**, check the email address on the payment and the list selections on the form.
