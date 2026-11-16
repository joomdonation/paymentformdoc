---
title: 'Anti Spam Settings'
published: true
media_order: anti-spam-settings.png
---

Payment Form includes built-in spam protection. Open the **Anti-Spam Settings** tab in **Configuration** to adjust these settings.

- **Honeypot Field Name** sets the name of the hidden field used to catch spam bots.
- **Honeypot Field Css Class** sets the CSS class for the honeypot field. We recommend keeping the default. If you use a class such as `my-custom-css-class`, add the following rule in the **Custom CSS** tab to hide the field from visitors.

    ```css
    .my-custom-css-class {
        display: none !important;
    }
    ```

- **Minimum Form Time (in Seconds)** sets how long visitors must wait before submitting a form. A minimum of 1 or 2 seconds can block automated submissions. Signed-in customers may also submit quickly if the form is prefilled from a previous submission. Leave this setting blank if you are unsure what minimum to use.
- **Force Form Time Check** rejects submissions that lack the form's timing field. It applies when **Minimum Form Time (in Seconds)** is greater than zero. If you use an older template override, make sure it includes the timing field before enabling this setting.
- **Maximum Form Submissions Per Session** limits submissions across all Payment Form forms in the same visitor session. For example, a limit of `10` allows up to 10 submissions in total. Leave it blank or set it to `0` to disable the limit.
- **Minimum Payment Amount** applies to the final total, after any discounts, taxes, and fees. For example, setting it to `5` blocks totals below 5 in the form's currency. Leave it blank or set it to `0` if you accept zero-amount or information-only submissions.

![Anti-spam settings](anti-spam-settings.png "anti-spam-settings")
