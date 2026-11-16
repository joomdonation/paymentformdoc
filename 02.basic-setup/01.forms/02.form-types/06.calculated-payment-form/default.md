---
title: 'Calculated Payment Form'
published: true
---

Use this form type when the amount depends on more than one input. Payment Form can combine quantities, selected options, fee formulas, and field dependencies to calculate the total.

## Example: training registration

A training provider charges 75 per attendee and offers an optional printed workbook for 12 per attendee. The workbook option appears only when the payer selects in-person attendance.

| Field | Name | Purpose | Fee setup |
| --- | --- | --- | --- |
| Number of attendees | `pf_quantity` | Payer enters the number of attendees | Not a fee field |
| Attendance Type | `attendance_type` | Payer chooses In-person or Online | Not a fee field |
| Training fee | `training_fee` | Charges for the attendees | **Hidden** field with default value `75`; **Fee Formula:** `[FIELD_VALUE] * [PF_QUANTITY]` |
| Printed workbook | `workbook` | Optional workbook for each attendee | **Fee Value:** `[PF_QUANTITY] * 12`; dependent on **Attendance Type: In-person** |

If the payer enters `3` attendees and selects the workbook, the training fee adds 225 and the workbook adds 36. The form total is 261 before later adjustments.

## Setup

1. Create the form and enter `0` for **Amount** when all pricing is calculated from fields.
2. Add a **Number** field named `pf_quantity`. Make it required and set a minimum value appropriate for the form.
3. Add a **Radio** field named `attendance_type` with **In-person** and **Online** as option values.
4. Add a **Hidden** fee field named `training_fee`, set its **Default Values** to `75`, and use `[FIELD_VALUE] * [PF_QUANTITY]` as its **Fee Formula**.
5. Add a **Checkboxes** field for the workbook. Set its option value to `workbook`, enable **Fee Field**, and set the matching **Fee Value** to `[PF_QUANTITY] * 12`.
6. On the workbook field, set **Depend On Field** to **Attendance Type** and select its **In-person** option under **Depend On Options**.
7. Test the form with one and several quantities, plus every option combination.

## Formula rules

- Refer to a field named `pf_quantity` as `[PF_QUANTITY]`. Field references must be uppercase and enclosed in square brackets.
- `[FIELD_VALUE]` means the value entered in the current fee field.
- `[FORM_AMOUNT]` means the base amount set on the form.
- `[PF_TOTAL_AMOUNT]` means the base amount plus ordinary custom field fees already calculated. Use it for a surcharge based on the current subtotal.
- A fee field hidden because its dependency condition is not met does not contribute to the total.

See [Custom Fee Fields](/basic-setup/custom-fields/custom-fee-fields) for the full formula reference and calculation order, and [Field Dependencies](/basic-setup/custom-fields/field-dependencies) for conditional-field setup.