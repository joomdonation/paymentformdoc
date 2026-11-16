---
title: 'Display a Single Form'
media_order: 'menu_item_types.png,Payment-Form-Form-Module.png'
---

Give a form its own page when visitors need a direct link to it. Use a module to put the form in a template position on an existing page, or embed it in an article to place it alongside the instructions visitors need to fill it in.

## Give a form its own page

For example, create a **Pay Membership Dues** menu item so members can go straight to the payment form from your site's navigation.

1. In the Joomla administrator area, open **Menus**, select the site menu where the link should appear, and click **New**.
2. Enter a **Menu Title**. Under **Menu Item Type**, click **Select** and choose **Payment Form → Form Modern Layout**.
3. In **Form**, select the form you want to display.
4. Leave **Number Columns**, **Form Format**, and **Show Fields Label** set to **Use Default** to inherit the form's settings, or change them for this menu item. See [Modern Form Layouts](/basic-setup/forms/modern-form-layouts) for examples.
5. Set **Status** to **Published**, choose the menu item's **Access** level, and save. Open the new page and check the form as a visitor would see it.

![Payment Form menu item types in Joomla](menu_item_types.png)

Use **Form Default Layout** when the page should follow the **Form Layout** selected in the form editor, including a custom layout. The **Inline Form Layout**, **2 Columns 2 Lines**, and **2 Columns Inline** menu item types are also available for existing setups.

## Show a form in a module position

Use **Payment Form - Form** when visitors should be able to fill in the form directly from an existing page, such as a short donation form on your homepage.

1. Go to **System → Site Modules**, click **New**, and select **Payment Form - Form**.
2. Enter a module title and select the form in **Form**.
3. Choose a **Position** in your site template. On **Menu Assignment**, choose the pages where the form should appear.
4. Set **Status** to **Published**, choose the module's **Access** level, and save. Open an assigned page and check that the form fits the position on desktop and mobile.

![Payment Form - Form module settings](Payment-Form-Form-Module.png)

## Embed a form in a Joomla article

Use **Content - Payment Form** when the form belongs within the article body, such as below workshop details and registration instructions.

1. Go to **System → Plugins** and enable **Content - Payment Form**.
2. Open **Components → Payment Form → Forms** and find the numeric **ID** of your form in the list.
3. Open the Joomla article and enter `{pmform FORM_ID}` on its own line where you want the form to appear. Replace `FORM_ID` with the numeric ID. For example, `{pmform 2}` displays form 2. Use one space between `pmform` and the ID.
4. Save the article and open it on your site. If the tag appears as text, check that the plugin is enabled and the tag matches the example.

For forms displayed through a module or article, set the layout in the form editor. If the form requires sign-in, set the menu item, module, or article to an access level that matches the intended audience. Once the form appears, [test a submission from that page](/basic-setup/forms/customize-form#test-the-form-on-your-site).

## Customize the completion page

To change the text shown after submission, edit the form's **Messages** tab. To give Payment Form's built-in completion page its own menu settings, create a published **Payment Form → Payment Complete** menu item and set **Display in Menu** to **No** on its **Link Type** tab. Customers reach this page through the checkout flow.

To send customers to a page you built separately, enter its address in the form's **Custom Payment Complete URL**. Test the result by submitting the form. See [Customize the confirmation](/basic-setup/forms/customize-form#customize-the-confirmation).
