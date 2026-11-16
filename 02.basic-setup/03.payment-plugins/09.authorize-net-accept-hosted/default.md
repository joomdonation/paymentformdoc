---
title: 'Authorize.net Accept Hosted'
media_order: 'webhook.png,plugin_parameters.png'
published: true
---

## Installation
When you purchase the payment plugin, you will receive a zip file called **os_pmf_authnetaccepthosted_unzip_first.zip**. Unzip the zip file, you will get the payment plugin file **os_pmf_authnetaccepthosted.zip** and three PHP files. 

- Go to **Payment Form** -> **Payment Plugins** to install the payment plugin **os_pmf_authnetaccepthosted.zip** as any other payment plugin. See [**Install Payment Plugin**](/basic-setup/payment-plugins#install-new-payment-plugin) for installation instructions if needed..
- For the three PHP files: **authaccepthosted_pmf_cancel.php**, **authaccepthosted_pmf_return.php**, **authaccepthosted_pmf_webhook.php**, please upload it to root folder of your site. If you use Admin Tools Pro htaccess marker, please make sure these three files are accessible by adding it to **Exceptions from Server Protection** section and re-generate the .htaccess file.

## Configuration

1. Login to your authorize.net account, access to **Account** -> **Account and API Settings**  -> **API Credentials and Keys**. Get API Login, Transaction Key (generate it if needed), Signature Key (generate if needed) and enter it to Associated parameters in the **os_authnetaccepthosted** payment plugin parameters.

![plugin_parameters](plugin_parameters.png "plugin_parameters")

2. Create a webhook in your Authorize.net account. Use `https://yourdomain.com/authaccepthosted_pmf_webhook.php` as the URL, replacing `https://yourdomain.com` with your site's base URL. Select **Authcapture Created (net.authorize.payment.authcapture.created)** as the event.

![webhook](webhook.png "webhook")
