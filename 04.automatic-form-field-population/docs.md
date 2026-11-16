---
title: 'Pre-populate Fields Data'
---

**Payment Form** has plugins to allow you to auto-fill form fields base on data stored in **Joomla User Profile** and third party extensions. Right now, the following third party extensions are supported: **Membership Pro**, **Community Builder**, **Jomsocial**. If users login and make payment using your form, the data stored in his profile (**Joomla User Profile or third party extensions profile**) will be used to fill-in form automatically so that he won't have to type the information again.

## Joomla User Profile 
To auto-fill form field use data from **Joomla User Profile** and Joomla User Custom Fields, please follow the steps below:
1. Go to **System** -> **Plugins**, find and enable the plugin **Payment Form - Userprofile**
2. Go to **Payment Form-> Custom Fields**, click on the custom field you want to auto-fill to edit, look at **Field Mappping** parameter, select the corresponding field in **Joomla User Profile** which will be used to fill-in this field. Save it.
3. Repeat step #2 for all other fields you want

## Membership Pro 
To auto-fill form field use data from **Membership Pro** user profile, please follow the steps below:
1. Go to **System** -> **Plugins**, find and enable the plugin **Payment Form - Membership Pro**
2. Go to **Payment Form-> Custom Fields**, click on the custom field you want to auto-fill to edit, look at **Field Mappping** parameter, select the corresponding field in **Membership Pro** which will be used to fill-in this field. Save it.
3. Repeat step #2 for all other fields you want

## Community Builder
This feature only works if you are using [**Community Builder**](http://extensions.joomla.org/extension/community-builder) extension on your site. If you don't use Community Builder extension, please ignore this section.

To auto-fill form field use data from **Community Builder**, please follow the steps below:

1. Go to **System** -> **Plugins**, find and publish the plugin **Payment Form - CB**
2. Go to **Payment Form-> Custom Fields**, click on the custom field you want to synchronize data to edit, look at **Field Mapping** property, select the corresponding field in **Community Builder** which will be used to fill-in this field. Save it.
3. Repeat step #2 for all other fields you want

## Jomsocial
This feature only works if you are using [**Jomsocial**](http://www.jomsocial.com/) extension on your site. If you don't use Jomsocial extension, please ignore this section.

To synchronize data with **Jomsocial**, please follow the steps below:

1. Go to **System** -> **Plugins**, find and publish the plugin **Payment Form - Joomsocial**
2. Go to **Payment Form -> Custom Fields**, click on the custom field you want to synchronize data to edit, look at **Field Mapping** property, select the corresponding field in **Jomsocial** which will be synchronized with this field. Save it.
3. Repeat step #2 for all other fields you want