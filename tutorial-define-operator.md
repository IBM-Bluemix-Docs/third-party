---

copyright:
  years: 2021
lastupdated: "2021-07-07"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, operator, validate, test, Red Hat OpenShift cluster, sample Node-RED Operator, Kubernetes cluster

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


# Defining your product details
{: #operator-define}
{: toc-content-type="tutorial"} 
{: toc-completion-time="15m"} 

This tutorial walks you through how to define the details of a sample Node-RED Operator as part of the process to onboard the software to the {{site.data.keyword.cloud}} catalog. By completing this tutorial, you learn how to provide your company and product information, create a test environment, set up access for your team, and provide your catalog entry and customer support details.
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

This tutorial uses a fictitious company that's called *Example Corp* that wants to onboard a sample Node-RED Operator to {{site.data.keyword.cloud}}. As you complete the tutorial, adapt each step to fit your product's details and desired structure.

## Before you begin
{: #operator-define-prereqs}

1. Verify that you're using a Pay-As-You-Go or Subscription account. To check which type of account you're using, go to **Manage** > **Account** > **Account settings** in the {{site.data.keyword.cloud_notm}} console. 
2. Contact us at kdmeyer@ibm.com to request access to {{site.data.keyword.cloud_notm}} Partner Center. In your email, include your account ID, which you can find on the Account settings page, and confirm that you understand the process to sell third-party software is a beta release. 

## Get set up to onboard the Operator
{: #operator-setup}
{: step}

Complete a few tasks that will help you start the onboarding process.

1. Go to the [Partner Center](https://cloud.ibm.com/partner-center/sell){: external} in the {{site.data.keyword.cloud_notm}} console, and click **Get started**.
2. Enter the name of your company, such as `Example Corp`, to identify your company, and click **Save**. 
3. Click **Create** your test environment, which includes a private catalog that you use to import the Operator ClusterServiceVersion (CSV) YAML file, enter `Sample Node-RED Operator Catalog` as the name of the private catalog, and click **Create**.
4. Click **Assign** to create an access group that's used to streamline assigning access to team members who might be helping you with the onboarding process. Enter `Sample Node-RED Operator Access` as the name of the access group, and click **Create**.
5. Click **Invite** to invite team members to your account and assign them to the access group that you created in the previous step. 
6. Click **Let's go** to start the oboarding process.

## Confirm the digital provider agreement
{: #operator-dpa}
{: step}

Third-party providers are required to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement, which sets the terms and conditions under which providers can onboard and sell products in {{site.data.keyword.cloud_notm}}. Or, third-party providers can upload a custom digital provider agreement in `.pdf`, `.doc`, or `.docx` file format. To complete the onboarding process, custom agreements must be reviewed and approved by {{site.data.keyword.IBM_notm}}.

Custom digital provider agreements must be reviewed and approved by {{site.data.keyword.IBM_notm}}, which increases the time it takes for you to complete the onboarding process. 
{: note}

For the purposes of this tutorial, complete the following steps to sign the {{site.data.keyword.IBM_notm}} Digital Provider Agreement. 

1. From the My products page in the {{site.data.keyword.cloud_notm}} Partner Center, click **Confirm your digital provider agreement** in the notification that explains you need to confirm your legal agreement with {{site.data.keyword.IBM_notm}}.
1. Click the **{{site.data.keyword.IBM_notm}} Digital Provider Agreement** link in the dialog to review the agreement. 
1. Return to the Partner Center, and select **I have read and agree to the {{site.data.keyword.IBM_notm}} Digital Provider Agreement**.
1. Click **Save**. 

## Enter the name of your Operator
{: #operator-name}
{: step}

1. From the Partner details tab, enter `Sample Node-RED Operator v1.0` as the product name.
2. Click **Save**.

## Define your catalog entry details
{: #operator-catalog}
{: step}

From the Catalog entry tab, provide certain product details that are displayed on your catalog entry when your Operator is published in the {{site.data.keyword.cloud_notm}} catalog.

1. Provide a logo by clicking **Add logo**, entering `http://svgur.com/i/TTP.svg`, and clicking **Save**.
2. Provide a product description by clicking **Enter description**, entering the following sample text, and clicking **Save**.

  `Node-RED is a programming tool for wiring together hardware devices, APIs, and online services in new and interesting ways.`
  
3. Set your catalog category by selecting `Developer Tools` and clicking **Save**.
4. Select **Third party** as the **Provider** type, and click **Save**.
5. Enter keywords that users might use when searching the catalog for your Operator, for example, `dev tools`, `node red`, and click **Save**.

## Define your support experience
{: #operator-support}
{: step}

To define your support experience, you provide details that help users understand how to get support if they encounter issues when using the Operator. You also describe how {{site.data.keyword.cloud_notm}} Support can collaborate with your support team on customer escalations.

1. From the Support tab, enter the URL to your support website, for example, `https://support.examplecorp.com/`, and click **Save**.
2. For the support response process, describe what users can expect when they contact your support team, as shown in the following example, and click **Save**.

  `Contact Example Corp Support online at https://support.examplecorp.com, by chat at https://support.examplecorp.com/chat, or by phone at https://support.examplecorp.com/phone. Support is available 24 hours a day, 7 days a week, 365 days a year and is provided in English and French.`
  
3. Enter or select all the countries in which support for your Operator is based, and click **Save**.
4. Describe the process that {{site.data.keyword.cloud_notm}} Support follows when customers escalate issues that are handled by your support team, as shown in the following example, and click **Save**. 

  `For client escalations, IBM Cloud support representatives should follow the escalation process described at https://support.examplecorp.com/ibmcloudescalations.`
  
5. Describe how {{site.data.keyword.cloud_notm}} Support can contact your support team, as shown in the following example, and click **Save**.

  `For support process discussions, IBM Cloud support leaders can reach out to the following Example Corp support leaders: Jane Doe (janedoe@examplecorp.com) and John Doe (johndoe@examplecorp.com).`


## Next steps
{: #operator-define-next}

Onboard the Operator to your private catalog and validate it's ready for use in the {{site.data.keyword.cloud_notm}} catalog. 

