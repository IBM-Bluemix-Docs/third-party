---

copyright:
  years: 2021
lastupdated: "2021-05-28"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, virtual server image, virtual machine image, image, vm, vsi, product details, catalog entry, support, pricing, BYOL, terraform, catalog

subcollection: third-party

content-type: tutorial
account-plan: paid
completion-time: 10m 

---

{:shortdesc: .shortdesc}
{:screen: .screen}  
{:codeblock: .codeblock}  
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:beta: .beta}
{:external: target="_blank" .external}
{:step: data-tutorial-type='step'} 


# Defining the product details of a virtual server image
{: #vsimage-define}
{: toc-content-type="tutorial"} 
{: toc-completion-time="10m"} 

This tutorial walks you through the steps for defining the details of a virtual server image with Terraform in {{site.data.keyword.cloud}} Partner Center. By completing this tutorial, you review and sign the {{site.data.keyword.IBM}} Digital Provider Agreement, and define your catalog entry, pricing model, and customer support experience. 
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own license or offer your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

This tutorial is one of four in a series that demonstrates how to onboard and publish a [sample virtual server image with Terraform](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/tree/v1.0){: external}. It uses a fictitious company that's called *Example Corp*. As you complete the tutorial, adapt each step to fit your product's needs.

## Before you begin
{: #vsimage-define-prereqs}

[Register your virtual server image in Partner Center](/docs/third-party?topic=third-party-vsimage-register).

## Confirm the digital provider agreement
{: #vsimage-dpa}
{: step}

Third-party providers are required to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement, which sets the terms and conditions under which providers can onboard and sell products in {{site.data.keyword.cloud_notm}}. Or, third-party providers have the option to upload a custom digital provider agreement in `.pdf`, `.doc` or `.docx` file format. To complete the onboarding process, custom agreements must be reviewed and approved by {{site.data.keyword.IBM_notm}}.

<!-- STAGING ONLY: until reviewed: 
Accepting the {{site.data.keyword.IBM_notm}} Digital Provider Agreement is much faster than using a custom digital provider agreement. Custom digital provider agreements must be reviewed and approved by IBM, which increases the time it takes for you to onboard. 
{: tip} -->

For the purposes of this tutorial, complete the following steps to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement. 

1. From the My products page in the {{site.data.keyword.cloud_notm}} Partner Center, click **Confirm your digital provider agreement** in the notification that explains you need to confirm your legal agreement with {{site.data.keyword.IBM_notm}}.
1. Click the **{{site.data.keyword.IBM_notm}} Digital Provider Agreement** link in the dialog to review the agreement. 
1. Return to the Partner Center, and select **I have read and agree to the {{site.data.keyword.IBM_notm}} Digital Provider Agreement**.
1. Click **Save**. 

## Provide the name of your virtual server image
{: #vsimage-name}
{: step}

1. From the Partner details tab, enter the name of your virtual server image, for example, `Example Corp Virtual Server Image 1.0.0`. Make sure the name meets the following requirements:
  
  * Use 60 characters or less.
  * Include the version.
  * Do not include the name of your company. You can include this information in your readme file.
  * Do not include any former product names. You can include this information as a keyword, in your readme file, or both.
  * Do not include `IBM Cloud`. 
  * Do not include details such as deployment targets, pricing, and so on. You can include this information in your readme file.   

1. Click **Save**.

## Define your catalog entry details
{: #vsimage-catalog}
{: step}

Each entry in the catalog consists a company or product logo, a short description that summarizes what the product is and its value, and other details. Because your catalog entry is visible to users as they browse the catalog, provide clear details that will help them find your virtual server image. 

1. From the Catalog entry tab, enter the URL to your company or product logo, such as `http://svgur.com/i/TTP.svg`, and click **Save**.
1. Provide a short description about your virtual server image, and click **Save**.
1. From the **Category** list, select an option that best fits how users might use your virtual server image. Categories are used to organize products in the catalog based on common solutions, function, or use.
1. Select **Third party** from the **Provider** list, and click **Save**.
1. Enter keywords that users might use when searching the catalog for your virtual server image, for example, **`virtual server`**, **`compute`**, and **`terraform`**, and click **Save**.

## Define your pricing model
{: #vsimage-pricing}
{: step}

{{site.data.keyword.cloud_notm}} support two pricing models: free or bring your own license (BYOL). With the free pricing model, users can deploy as many instances with no additional software charges incurred. With the BYOL pricing model, {{site.data.keyword.cloud_notm}} doesn't charge users for the usage of the software, and the third-party provider is responsible for licensing entitlement and enforcement. 

For the purposes of this tutorial, complete the following steps to add a BYOL pricing plan. 

1. From the Pricing tab, click **Pricing plans**.
1. Click **Add plan**, and select **BYOL**.
1. On the Add pricing plan panel, enter the name, URL, and description of the license, for example: 

  * Name: `BYOL for Example Corp Virtual Server Image 1.0.0`
  * URL: `byol.vsimage.examplecorp.html`
  * Description: `This BYOL license is required for the installation and use of the Example Corp Virtual Server Image.`

## Define your customer support experience
{: #vsimage-support}
{: step}

Provide details that help users understand how to get help and support when using the virtual server image.

1. From the Support tab, enter the URL to your support website, for example, `https://support.examplecorp.com/`, and click **Save**.
2. Describe what users can expect when they contact your support team, as shown in the following example, and click **Save**.

  `This product is provided and supported by Example Corp. If you encounter problems, you can open a support issue with the Example Corp support team. Responses to support issues are typically provided in approximately 1 to 2 business days.`
  
3. Enter a description of how {{site.data.keyword.cloud_notm}} can contact your support team, as shown in the following example, and click **Save**.

  `For client escalation, IBM Cloud Support contacts our escalation desk at 1-555-555-5555, speaks to a Duty Manager, and reports the client name and contact information.`
  
4. Enter a description of how users can get in touch with your support team, as shown in the following example, and click **Save**.

  `If you run into issues, you can contact Example Corp by chat at https://support.examplecorp.com/chat or by phone at https://support.examplecorp.com/phone 24 hours a day, 7 days a week.`

5. Enter or select all the countries in which support for your virtual server image is based, and click **Save**.

## Next steps
{: #vsimage-define-next}

[Onboard your Terraform template to your private catalog](/docs/third-party?topic=third-party-vsimage-onboard). 







