---
title: 'Invoice Settings'
published: true
media_order: invoice-settings.png
---

Set **Activate Invoice Feature** to **Yes** to generate PDF invoices for payments with a positive amount.

In **System → Plugins**, check that **Payment Form - Invoice Generator** is enabled. It assigns the invoice number used for PDF downloads and email attachments.

![Invoice settings](invoice-settings.png "invoice-settings")

## When invoices are issued

- **Only Generate Invoice For Paid Payment** lets you defer invoices for pending offline payments until you mark them as **Paid**. Set it to **No** if you want Payment Form to generate an invoice when the customer submits an offline payment.
- **Send Invoice To Customers** attaches the PDF to the customer's confirmation email. If you defer the invoice for an offline payment, Payment Form attaches it to the approval email. Signed-in customers can also download available invoices from the [Payment History](/frontend-items/payment-history) page if you add it to your site.
- **Send Invoice To Admin** attaches a copy to the administrator's payment notification when an invoice is available at the time the notification is sent.

## Numbering and appearance

- **Invoice Start Number** sets the first invoice number. If invoices already exist, Payment Form uses the higher of this setting and the highest existing invoice number plus one.
- **Invoice Prefix** adds text before the number. **Invoice Number Length** sets the minimum number of digits and pads shorter numbers with leading zeros. For example, a start number of `100`, a prefix of `INV-`, and a length of `5` produce `INV-00100`.
- **Invoice Format** controls the default PDF template. Replace the logo and company details with your own. A form can specify its own invoice template.
- **PDF Font** selects the font for generated invoices. If characters appear missing or as boxes, choose a font that supports the characters used in your invoices.
