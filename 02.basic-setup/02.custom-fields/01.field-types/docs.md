---
title: 'Supported Field Types'
taxonomy:
    category:
        - docs
---

Payment Form includes the following 22 custom field types:

1. **Text** — A single-line text input.
2. **Email** — An email address input.
3. **Url** — A URL input.
4. **Number** — A numeric input.
5. **Tel** — A telephone number input.
6. **Password** — A password input.
7. **Hidden** — A value submitted with the form without showing an input to the payer.
8. **Range** — A range slider.
9. **Textarea** — A multi-line text input.
10. **List** — A dropdown. Set **Multiple** to **Yes** to allow more than one selection.
11. **Checkboxes** — A group of options that can be selected together.
12. **Radio** — A group of options where only one can be selected.
13. **Date** — A date picker.
14. **Time** — A time input.
15. **Heading** — Displays the field title as a heading; it does not collect a value.
16. **Message** — Displays the field's **Description** as text on the form.
17. **File** — Lets the payer upload a file. Allowed extensions are controlled by the **Allowed File Types** configuration setting.
18. **Countries** — A dropdown of published countries.
19. **States** — A dropdown of states for the selected country.
20. **Signature** — A signature input.
21. **Editor** — A rich-text editor.
22. **SQL** — A dropdown whose options come from a SQL query in **Default Values**. The query must return two columns named `value` and `text`. For example:

    ```sql
    SELECT name AS value, name AS text
    FROM #__pf_countries
    WHERE published = 1
    ORDER BY name
    ```

### Country and state fields

Use no more than one **Countries** field and one **States** field on a form. They work together: changing the country updates the state options. If the form has a **States** field but no **Countries** field, the options come from the **Default Country** selected in Payment Form configuration.
