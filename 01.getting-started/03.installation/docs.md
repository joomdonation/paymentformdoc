---
title: 'Installation & Upgrade'
taxonomy:
    category:
        - docs
media_order: 'uninstall.png,dashboard.png,plug_cb_pmhistory.zip'
---

## Installation

After you purchase Payment Form, you'll receive an email with `payment_form_unzip_first.zip`. Extract that file to get `com_pmform.zip` and `plug_cb_pmhistory.zip`.

### Install the component, modules and plugins

The `com_pmform.zip` package contains the Payment Form component, modules, and Joomla plugins.

1. Log in to the Joomla administrator area with a Super User account.
2. Go to **System → Install → Extensions**.
3. Select `com_pmform.zip`.
4. Click **Upload & Install**.

After installation, Joomla opens the Payment Form dashboard, where you can start configuring the extension.

![Payment Form dashboard](dashboard.png)

## Install the CB Payment History plugin

If your site uses Community Builder, you can install the optional CB Payment History plugin through Community Builder's plugin manager.

1. Download [plug_cb_pmhistory.zip](plug_cb_pmhistory.zip) or use the copy from the purchase ZIP file.
2. Log in to the Joomla administrator area.
3. Go to **Components → Community Builder → Plugins Management**.
4. Click **Install Plugin**.
5. Select `plug_cb_pmhistory.zip`.
6. Click **Upload and Install**.

## Install Sample Data

On a new installation, you can use the sample data from our demo site to see how Payment Form is set up. Log in to the Joomla administrator area and open the following URL.

`https://domain.com/administrator/index.php?option=com_pmform&task=tool.setup_sample_data`

Replace `https://domain.com/administrator` with the URL of your site's Joomla administrator area.

### Update

You can update Payment Form using Joomla's extension updater.

1. Get your Download ID from [Download IDs](https://joomdonation.com/download-ids.html) in your JoomDonation account.
2. In Joomla, go to **Payment Form → Configuration** and enter it in the **Download ID** field.

When a new version is available, Joomla displays a notice in the administrator area or on the Payment Form dashboard. Follow the link in the notice to update Payment Form from within your site.

Use a unique Download ID for each site. You can use that site's Download ID for all JoomDonation products installed on it.

## Update Manually

If you need to update Payment Form manually, download the latest version from [My Downloads](https://joomdonation.com/my-downloads.html) and follow the installation steps above to install the new package.

## Move data from one site to a new site

1. In phpMyAdmin, export the Payment Form tables from the old site's database. Their names start with the Joomla database prefix followed by `pf_`.
2. If the sites use different database table prefixes, open the exported SQL file in a text editor and change the prefixes in the table names to match the new site.
3. Use phpMyAdmin to import the tables into the new site's database.
4. Reinstall the latest version of Payment Form on the new site to update the database schema.

## Uninstall

1. Log in to the Joomla administrator area with a Super User account.
2. Go to **System → Manage → Extensions**.
3. Choose **Package** from the **Select Type** filter.
4. Select the checkbox next to **Payment Form Package**.
5. In the toolbar, choose **Actions → Uninstall**.

![Uninstalling the Payment Form package](uninstall.png "uninstall")

Joomla uninstalls the Payment Form component, modules, and plugins.

>>>>> Uninstalling Payment Form keeps its database tables so your data is available if you reinstall it. To permanently delete the data, use phpMyAdmin to drop the tables whose names start with your Joomla database prefix followed by `pf_`.
