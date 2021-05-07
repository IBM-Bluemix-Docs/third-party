---

copyright:
  years: 2021
lastupdated: "2021-05-06"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, virtual server image, virtual machine image, image, vm, vsi, publish, Terraform, tutorial, sample

subcollection: third-party

content-type: tutorial
account-plan: paid
completion-time: 30m 

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


# Publishing a sample virtual server image to the {{site.data.keyword.cloud_notm}} catalog
{: #vsimage-publish}
{: toc-content-type="tutorial"} 
{: toc-completion-time="30m"} 

This tutorial walks you through how to publish a sample virtual server image to {{site.data.keyword.cloud}}. By completing this tutorial, you learn how to submit a request to publish the sample virtual server image, and then publish it to the {{site.data.keyword.cloud}} catalog.
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or offer your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

This tutorial is one of four in a series that demonstrates how to onboard and publish a [sample virtual server image with Terraform](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/tree/v1.0){: external}. As you complete the tutorial, adapt each step to fit your product's needs.

## Before you begin
{: #vsimage-publish-prereqs}

Complete the previous tutorials in the series:

* [Registering a sample virtual server image in Partner Center](/docs/third-party?topic=third-party-vsimage-register)
* [Defining the product details](/docs/third-party?topic=third-party-vsimage-define)
* [Onboarding a sample virtual server image to your private catalog](/docs/third-party?topic=third-party-vsimage-onboard)

## Request to publish the sample virtual server image
{: #vsimage-publish-submit}
{: step}

1. In the {{site.data.keyword.cloud_notm}} console, click the **Menu** icon ![Menu icon](../icons/icon_hamburger.svg) > **Partner Center > Sell > My Products**.
1. Select **isv-vsi-product-deploy-sample v1.0.0** from the list. 
1. From the Onboarding checklist, click **Request Approval**. 
1. Select **1.0.0** as the version that you want to publish > **I affirm that my company is authorized to use all materials**. 
1. Click **Request Approval**.

At this point, your publishing request is reviewed by {{site.data.keyword.cloud_notm}} to ensure the required details, such as the product name, catalog entry, pricing model, and support experience, are complete and accurate. When your request is approved, you receive an email notifiying you that you can publish the sample virtual server image to the catalog. 

If updates are required, you'll receive a separate email with details about the required updates. After you address all review feedback, you can submit another publishing request.
{: note} 

## Publish the sample virtual server image
{: #vsimage-publish-submit}
{: step}

1. Navigate to the Partner Center in the {{site.data.keyword.cloud_notm}} console by clicking the link in the email that you received notifiying you that your publishing request was approved.
1. Click **Publish to catalog**.
1. Verify that the sample virtual server image is published. Go to the [catalog](https://cloud.ibm.com/catalog){: external}, select **Software**, and search for it by typing `isv-vsi-product-deploy-sample v1.0.0`. 

## Next steps
{: #vsimage-publish-next}

Even though you published the sample virtual server image to the catalog, it's not yet publicly available to other accounts. Use a REST API to make the image public so that users can then use it to create virtual server instances. For more information, see [Update the visibility of your image](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample#update-the-visibility-of-your-image-patch-api){: external}.

