---
title: 'Stripe Checkout'
media_order: signing_secret.png
published: true
---

## Installation
When you purchase the payment plugin, you will receive a zip file called **os_pmf_stripecheckout_unzip_first.zip**. Unzip that file, you will get the file os_pmf_stripecheckout.zip. Go to **Payment Form** -> **Payment Plugins** to install it as any other payment plugin. See [https://docs.joomdonation.com/paymentform/basic-setup/payment-plugins#install-new-payment-plugin/basic-setup/payment-plugins#install-new-payment-plugin](/basic-setup/payment-plugins#install-new-payment-plugin) for installation instructions if needed.

## Configuration

1. Follow instructions [ https://stripe.com/docs/keys#api-keys]( https://stripe.com/docs/keys#api-keys) , get your Stripe API Keys and enter it into the payment plugin parameters.

2. Follow instructions at [https://stripe.com/docs/webhooks/setup#add-endpoint-dashboard](https://stripe.com/docs/webhooks/setup#add-endpoint-dashboard), add the webhook URL below to your Stripe account:

**https://domain.com/index.php?option=com_pmform&task=payment_confirm&payment_method=os_stripecheckout**

(Of course, need to replace **https://domain.com/** with your website url)

Select the event **checkout.session.completed** for that webhook URL.

3. After setting up webhook, you need to get **Signing secret** of the webhook URL, and enter it into **Signing Secret** parameter of the payment plugin. In the webhook URL setting, click on Reveal button to get it (see the below screenshot)

![signing_secret](signing_secret.png "signing_secret")