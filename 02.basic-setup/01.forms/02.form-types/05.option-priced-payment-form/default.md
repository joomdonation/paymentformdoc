---
title: 'Option-Priced Payment Form'
published: true
---

Use this setup when each ticket, plan, product, or add-on has its own price. Payment Form adds the fees for the options the payer selects.

## Example conference registration

Create a required **Ticket Type** field and an optional **Add-ons** field. The table shows what to enter for each option.

| Field | Options Value | Options Text | Fee Values |
| --- | --- | --- | ---: |
| Ticket Type | `standard` | Standard ticket (+120) | `120` |
| Ticket Type | `premium` | Premium ticket (+180) | `180` |
| Add-ons | `workshop` | Workshop (+50) | `50` |
| Add-ons | `lunch` | Lunch (+15) | `15` |

With a base amount of `0`, a Standard ticket and both add-ons give a subtotal of `120 + 50 + 15 = 185`.

## Setup

1. [Create the form](/basic-setup/forms/add-new-form) and set **Amount** to `0`. Enter a base amount if every payer should also pay a fixed fee.
2. In **Custom Fields**, create **Ticket Type** as a **Radio** field or a **List** with **Multiple** set to **No**. Set **Required** to **Yes**.
3. Create **Add-ons** as a **Checkboxes** field or a **List** with **Multiple** set to **Yes**. Set **Required** to **No** and leave **Default Values** blank if add-ons should start unselected.
4. Assign both fields to this form and set **Fee Field** to **Yes**. For each field, enter one line per option in **Options Value**, **Options Text**, and **Fee Values**. Keep the lines in the same order and leave **Fee Formula** blank.
5. Select the form's payment methods. [Display the form](/frontend-items/display-a-single-form) and check the total for each ticket, with and without add-ons.

Use [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) for a complete configuration example.
