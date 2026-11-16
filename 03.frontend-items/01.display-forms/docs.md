---
title: 'Display a List of Forms'
taxonomy:
    category:
        - docs
media_order: 'Payment-Form-Forms-List.png,Payment-Form-Forms-List-Module.png'
---

Visitors can open a payment form by clicking its title in either list.

## Create a Forms List page

Use a dedicated page when visitors need to choose what to pay for. For example, a **Club Payments** page could list forms for annual dues, event fees, and donations.

1. In the Joomla administrator area, open **Menus**, select the site menu where the link should appear, and click **New**.
2. Enter a **Menu Title**. Under **Menu Item Type**, click **Select** and choose **Payment Form → Forms List**.
3. Configure the list using the settings below. Set **Status** to **Published**, choose the menu item's **Access** level, and save.
4. Open the new page on your site and click each title to verify that it opens the expected form.

| Setting | What it controls |
| --- | --- |
| **Forms** | Select the forms for this page, or leave the selection empty to include all available forms. |
| **Show Amount Columns** | Controls the **Amount** column, which shows the base amount saved on each form. The setting defaults to **Yes**. Choose **No** for a list of donations, payer-entered amounts, or other forms where the total is determined when the visitor fills in the form. Check the page after saving to confirm that the column appears as intended. |
| **Intro Text** | Appears above the table. Use it to explain which form visitors should choose. |

![Forms List page showing linked form titles below the introductory text](Payment-Form-Forms-List.png)

## Show form links in a module position

Use the module for a compact list of links on one or more existing pages. For example, place links to your payment forms in the sidebar of a member information page.

1. Go to **System → Site Modules**, click **New**, and select **Payment Form - Forms List**.
2. Enter a module title. Under **Forms**, select the forms to include or leave the selection empty. Set **Number Forms** to the maximum number of links to show. The default is **10**.
3. Choose a **Position** in your site template. On **Menu Assignment**, choose the pages where the list should appear.
4. Set **Status** to **Published**, choose the module's **Access** level, and save. Visit an assigned page to check the list and its links.

![Forms List module with a bulleted list of links](Payment-Form-Forms-List-Module.png)

Both lists show only published forms within their publishing dates that the visitor has permission to open. If a form is missing, check its [publishing and access settings](/basic-setup/forms/add-new-form#general) and the **Forms** selection. For the module, also check **Number Forms** and **Menu Assignment**.
