---
title: 'Form Types'
---

Payment Form can collect information, accept a fixed payment, let the payer choose an amount, or calculate a total from their selections. Start with the form type that matches how the amount should be determined.

| If you need to… | Use this guide |
| --- | --- |
| Collect information without taking a payment | [Information Collection Form](/basic-setup/forms/form-types/information-collection-form) |
| Charge the same amount to every payer | [Fixed Amount Payment Form](/basic-setup/forms/form-types/fixed-amount-payment-form) |
| Let each payer enter the amount | [Payer-Entered Amount Form](/basic-setup/forms/form-types/payer-entered-amount-form) |
| Price a form from ticket types, upgrades, or add-ons | [Option-Priced Payment Form](/basic-setup/forms/form-types/option-priced-payment-form) |
| Calculate prices from quantities, selections, and conditions | [Calculated Payment Form](/basic-setup/forms/form-types/calculated-payment-form) |

All payment forms use the same sequence:

```text
Base form amount + custom field fees = form total
```

Payment Form then applies a late-payment fee, coupon discount, tax, and payment-method processing fee when those features are configured. See [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) for the calculation rules and formula reference.

After choosing a form type, create the form, assign its custom fields, choose the available payment methods, and test a complete submission before publishing it.