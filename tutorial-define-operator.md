---

copyright:
  years: 2021
lastupdated: "2021-04-01"

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

1. In the {{site.data.keyword.cloud_notm}} console, click the Menu icon ![Menu icon](../icons/icon_hamburger.svg) > **Partner Center** > **Start selling** > **Get started**.
2. Enter the name of your company, such as `Example Corp`, to identify your company, and click **Save**. 
3. Click **Create** your test environment, which includes a private catalog that you use to import the Operator ClusterServiceVersion (CSV) YAML file, enter `Sample Node-RED Operator Catalog` as the name of the private catalog, and click **Create**.
4. Click **Assign** to create an access group that's used to streamline assigning access to team members who might be helping you with the onboarding process. Enter `Sample Node-RED Operator Access` as the name of the access group, and click **Create**.
5. Click **Invite** to invite team members to your account and assign them to the access group that you created in the previous step. 
6. Click **Let's go** to start the oboarding process.

## Confirm the digital provider agreement
{: #operator-dpa}
{: step}

1. From the My products tab, click **OK** in the notification that explains you need to confirm your legal agreement with {{site.data.keyword.IBM_notm}}.
2. Review the [IBM Digital Provider Agreement](https://mp.s81c.com/pwb-production/000002-partner-docs/PartnerAgreement/5.0.0/IBM.Digital.Provider.Agreement.Referral.Only.Terms.03062020.clean.pdf){: external}.
3. Return to the Partner Center, and select **I understand and confirm that I have signed the IBM Digital Provider Agreement**.
4. Click **Save**. 

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

## Define your customer support experience
{: #operator-support}
{: step}

From the Support tab, provide details that help users understand how to get help and support when using the Operator.

1. In the **Support site URL** field, enter the URL to your support website, for example, `https://support.examplecorp.com/`, and click **Save**.
2. In the **Support response process** field, describe what users can expect when they contact your support team, as shown in the following example, and click **Save**.

  `This product is provided and supported by Example Corp. If you encounter problems, you can open a support issue with the Example Corp support team. Responses to support issues are typically provided in approximately 1 to 2 business days.`
  
3. In the **{{site.data.keyword.cloud_notm}} Support response process** field, enter a description of how {{site.data.keyword.cloud_notm}} can contact your support team, as shown in the following example, and click **Save**.

  `For client escalation, IBM Cloud Support contacts our escalation desk at 1-555-555-5555, speaks to a Duty Manager, and reports the client name and contact information.`
  
4. In the **Support contacts** field, enter a description of how users can get in touch with your support team, as shown in the following example, and click **Save**.

  `If you run into issues, you can contact Example Corp by chat at https://support.examplecorp.com/chat or by phone at https://support.examplecorp.com/phone 24 hours a day, 7 days a week.`

5. From the **Support location** list, enter or select all the countries in which support for your product is available, for example, **United States** and **Canada**, and click **Save**.


## Next steps
{: #operator-define-next}

Onboard the Operator to your private catalog and validate it's ready for use in the {{site.data.keyword.cloud_notm}} catalog. 

