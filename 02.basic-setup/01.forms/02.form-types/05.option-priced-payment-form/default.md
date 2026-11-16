---
title: 'Option-Priced Payment Form'
published: true
---

Use this form type when the payer chooses a ticket, plan, product, or add-on and each choice has a known price. Payment Form maps the selected option to the matching line in **Fee Values**.

## Example: conference registration

The form has a required ticket-type field and optional add-ons:

| Field | Type | Selected option | Added fee |
| --- | --- | --- | ---: |
| Ticket Type | Radio | Standard ticket | 120 |
| Add-ons | Checkboxes | Workshop | 50 |
| Add-ons | Checkboxes | Lunch | 15 |

If the payer chooses a Standard ticket and both add-ons, the form total is 185 before discounts, tax, and payment-method fees.

## Setup

1. Create the form and set its **Amount** to `0` when all pricing comes from selections. Enter a base amount if every payer should also pay a fixed fee.
2. Add a **Radio** or single-select **List** field for the required choice, such as ticket type.
3. Enter one stored option per line in **Options Value**, for example `standard`, `premium`, and `vip`.
4. Enter matching labels in **Options Text**, such as `Standard Ticket (+120)`.
5. Set **Fee Field** to **Yes** and enter the corresponding amounts in **Fee Values**, one per line in the same order.
6. Add **Checkboxes** or a multiple-select **List** for optional add-ons, following the same value-to-fee mapping.
7. Choose payment methods, publish the form, and test every selection combination.

## How Payment Form calculates it

- A **Radio** field or single-select **List** adds the fee for one selected option.
- **Checkboxes** and a multiple-select **List** add the fees for all selected options.
- Each line in **Fee Values** belongs to the option on the same line in **Options Value**. Keep the lists in the same order.

Use [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) for a complete configuration example.