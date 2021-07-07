---

copyright:
  years: 2021

lastupdated: "2021-07-07"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, operator, validate, test, Red Hat OpenShift cluster, bundle, Kubernetes cluster, product details, catalog listing, support, pricing, BYOL

subcollection: third-party

content-type: tutorial
account-plan: paid
completion-time: 15m 

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

# Defining the product details of your Operator bundle from the {{site.data.keyword.redhat_notm}} Certified registry
{: #bundle-define}
{: toc-content-type="tutorial"} 
{: toc-completion-time="10m"} 

This tutorial walks you through the steps for defining the details of an Operator bundle in {{site.data.keyword.cloud}} Partner Center. By completing this tutorial, you review and sign the {{site.data.keyword.IBM}} Digital Provider Agreement, and define your catalog entry, pricing model, and customer support experience. 
{: shortdesc}

The process to sell third-party software is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you have questions, contact us at kdmeyer@ibm.com.
{: beta}

This tutorial is one of four in a series that demonstrates how to onboard and publish a sample Operator bundle from the {{site.data.keyword.redhat_full}} {{site.data.keyword.openshiftshort}} Certified registry. It uses a fictitious company that's called *Example Corp*. As you complete the tutorial, adapt each step to fit your product's needs.

## Before you begin
{: #bundle-define-prereqs}

[Register your Operator bundle in Partner Center](/docs/third-party?topic=third-party-bundle-register).

## Confirm the digital provider agreement
{: #bundle-dpa}
{: step}

Third-party providers are required to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement, which sets the terms and conditions under which providers can onboard and sell products in {{site.data.keyword.cloud_notm}}. Or, third-party providers can upload a custom digital provider agreement in `.pdf`, `.doc`, or `.docx` file format. 

Custom digital provider agreements must be reviewed and approved by {{site.data.keyword.IBM_notm}}, which increases the time it takes for you to complete the onboarding process. 
{: note}

For the purposes of this tutorial, complete the following steps to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement. 

1. From the My products page in the {{site.data.keyword.cloud_notm}} Partner Center, click **Confirm your digital provider agreement** in the notification that explains you need to confirm your legal agreement with {{site.data.keyword.IBM_notm}}.
1. Click the **{{site.data.keyword.IBM_notm}} Digital Provider Agreement** link in the dialog to review the agreement. 
1. Return to the Partner Center, and select **I have read and agree to the {{site.data.keyword.IBM_notm}} Digital Provider Agreement**.
1. Click **Save**. 

## Enter the name of your Operator bundle
{: #bundle-name}
{: step}

From the Partner details tab, enter the name of your Operator bundle as it appears in the {{site.data.keyword.redhat_notm}} registry in the product name field. 

1. From the Partner details tab, enter the name of your Operator bundle. For example, for the purposes of this tutorial, you can enter `Akka Cluster Operator`.
2. Click **Save**.

## Define your catalog entry details
{: #bundle-catalog}
{: step}

From the Catalog entry tab, provide certain product details that are displayed on your catalog entry when your Operator bundle is published in the {{site.data.keyword.cloud_notm}} catalog.

1. From the Catalog entry tab, click **Add logo**, enter the URL to your company or product logo, such as `http://svgur.com/i/TTP.svg`, and click **Save**.
2. Provide a short description by clicking **Enter description**, entering the description, and clicking **Save**. For the purposes of this tutorial, you can enter the following text.

  `This Operator is a developer tool.`
  
3. Set your catalog category by selecting `Developer Tools` and clicking **Save**.
4. Select **Third party** as the **Provider** type, and click **Save**.
5. Enter keywords that users might use when searching the catalog for your Operator bundle, for example, **`dev tools`** and **`operator`**, and click **Save**.

## Defining your pricing model
{: #bundle-pricing}

From the pricing tab, define the pricing model for your Operator bundle. Currently, the {{site.data.keyword.cloud_notm}} catalog supports free plans and bring your own license (BYOL). For the purposes of this tutorial, complete the following steps to make the Operator bundle free. 

1. From the pricing tab, select **Free**. 

## Define your support experience
{: #bundle-support}
{: step}

To define your support experience, you provide details that help users understand how to get support if they encounter issues when using the Operator bundle. You also describe how {{site.data.keyword.cloud_notm}} Support can collaborate with your support team on customer escalations.

1. From the Support tab, enter the URL to your support website, for example, `https://support.examplecorp.com/`, and click **Save**.
2. For the support response process, describe what users can expect when they contact your support team, as shown in the following example, and click **Save**.

  `Contact Example Corp Support online at https://support.examplecorp.com, by chat at https://support.examplecorp.com/chat, or by phone at https://support.examplecorp.com/phone. Support is available 24 hours a day, 7 days a week, 365 days a year and is provided in English and French.`
  
3. Enter or select all the countries in which support for your Operator bundle is based, and click **Save**.
4. Describe the process that {{site.data.keyword.cloud_notm}} Support follows when customers escalate issues that are handled by your support team, as shown in the following example, and click **Save**. 

  `For client escalations, IBM Cloud support representatives should follow the escalation process described at https://support.examplecorp.com/ibmcloudescalations.`
  
5. Describe how {{site.data.keyword.cloud_notm}} Support can contact your support team, as shown in the following example, and click **Save**.

  `For support process discussions, IBM Cloud support leaders can reach out to the following Example Corp support leaders: Jane Doe (janedoe@examplecorp.com) and John Doe (johndoe@examplecorp.com).`


## Next steps
{: #bundle-define-next}

[Onboard your Operator bundle](/docs/third-party?topic=third-party-bundle-onboard) to your private catalog and validate it's ready for use in the {{site.data.keyword.cloud_notm}} catalog. 

