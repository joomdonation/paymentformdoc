---
title: 'Automatic Form Field Population'
---

When a signed-in user opens a payment form, Payment Form can prefill fields with values from the user's Joomla profile or from Membership Pro, Community Builder, or JomSocial. Enable the integration plugin for your profile source, then map each Payment Form field you want to prefill to its corresponding profile field.

## Enable the plugin for your profile source

In the Joomla administrator, go to **System → Plugins** and enable the Payment Form plugin for your profile source. If several profile integration plugins are enabled, **Field Mapping** shows the fields from the first plugin that supplies them. To choose the source, leave only its Payment Form profile integration plugin enabled.

| Profile source | Plugin to enable | Requirements |
| --- | --- | --- |
| Joomla user profile and user custom fields | **Payment Form - Userprofile** | Enable Joomla's **User - Profile** plugin to map its built-in profile fields. Published Joomla user custom fields are available through **Payment Form - Userprofile**. |
| Membership Pro | **Payment Form - Membership Pro** | Membership Pro must be installed on the same site. |
| Community Builder | **Payment Form - CB** | Community Builder must be installed on the same site. |
| JomSocial | **Payment Form - Joomsocial** | JomSocial must be installed on the same site. |

## Map the fields

1. Go to **Components → Payment Form → Custom Fields** and open the Payment Form field you want to prefill.
2. Under **Field Mapping**, select the profile field that supplies the value. For example, to prefill a **Billing City** field from the Joomla user profile, select `city`.
3. Set **Populate From Previous Payment** to **Yes**. This setting also allows the field to display a value from the mapped profile field.
4. Save the field and repeat these steps for each field you want to prefill.

If **Field Mapping** is missing, check that the integration plugin is enabled and that the profile source has fields available to map.

## Test the form

Sign in to the site with a test account that has values saved in the mapped profile fields and no previous Payment Form submissions. Open the form and check that the expected values appear before you submit it.
