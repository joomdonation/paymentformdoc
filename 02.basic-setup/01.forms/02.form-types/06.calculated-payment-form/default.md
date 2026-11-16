---
title: 'Calculated Payment Form'
published: true
---

Use this setup when prices depend on quantities or other field values. You can also show a priced option only when a condition is met.

## Example training registration

A training provider charges 75 per attendee and offers an optional printed workbook for 12 per attendee. The workbook option appears only when the payer selects in-person attendance.

| Field | Name | Type | Fee setup |
| --- | --- | --- | --- |
| Number of attendees | `pf_quantity` | **Number** | **Fee Field** set to **No** |
| Attendance type | `attendance_type` | **Radio** | **Fee Field** set to **No** |
| Training fee | `training_fee` | **Hidden** | **Default Values** set to `75`, **Fee Formula** set to `[FIELD_VALUE] * [PF_QUANTITY]` |
| Printed workbook | `workbook` | **Checkboxes** | **Fee Values** set to `[PF_QUANTITY] * 12` for the workbook option |

For three in-person attendees with workbooks, the subtotal is `(3 × 75) + (3 × 12) = 261`. For three online attendees, it is `3 × 75 = 225`.

## Setup

1. [Create the form](/basic-setup/forms/add-new-form) and set **Amount** to `0`. Create the following fields in **Custom Fields** and assign them to this form.
2. Make **Number of attendees** required and set **Min** and **Step** to `1` for whole quantities. Set **Default Values** to `1` so the form starts with one attendee.
3. Make **Attendance type** required. Enter `in_person` and `online` as separate lines in **Options Value**, with **In-person** and **Online** on the matching lines in **Options Text**.
4. Set **Fee Field** to **Yes** for **Training fee**. Enter the default value and formula from the table.
5. For **Printed workbook**, set **Options Value** to `workbook` and **Options Text** to `Include a printed workbook`. Set **Fee Field** to **Yes**, enter the expression in **Fee Values**, and leave **Fee Formula** blank. Leave **Required** set to **No**.
6. On **Printed workbook**, set **Depend On Field** to **Attendance type** and select **In-person** under **Depend On Options**.
7. Select the form's payment methods and [display the form](/frontend-items/display-a-single-form). Test several quantities, then select the workbook and switch to **Online** to verify that its fee is removed.

## Formula rules

- Refer to a field named `pf_quantity` as `[PF_QUANTITY]`. Field references must be uppercase and enclosed in square brackets.
- `[FIELD_VALUE]` uses the current fee field's value. In this example it uses the hidden field's default of `75`.
- `[FORM_AMOUNT]` means the base amount set on the form.
- `[PF_TOTAL_AMOUNT]` can be used in **Fee Formula** for a surcharge based on the subtotal of the base amount and the fees already calculated.
- A fee field contributes only when its field dependency conditions are met.

See [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) for the full formula reference and calculation order, and [Field Dependencies](/basic-setup/custom-fields/field-dependencies) for conditional-field setup.
