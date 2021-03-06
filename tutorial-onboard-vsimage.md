---

copyright:
  years: 2021
lastupdated: "2021-06-07"

keywords: onboard software, Terraform, third-party software, sell on IBM Cloud, partner center, virtual server image, virtual machine image, image, vm, vsi, validate, test, VSI image, VM image

subcollection: third-party

content-type: tutorial
services: cloud-object-storage, vpc
account-plan: paid
completion-time: 45m 

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


# Onboarding a virtual server image with Terraform to a private catalog
{: #vsimage-onboard}
{: toc-content-type="tutorial"}
{: toc-services="cloud-object-storage, vpc"} 
{: toc-completion-time="45m"} 

This tutorial walks you through how to onboard a virtual server image with Terraform to a private catalog. By completing this tutorial, you learn how to import the virtual server image from a GitHub repository, configure the deployment and other details, and validate that you can deploy the image to a target {{site.data.keyword.vpc_full}} (VPC). 
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or offer your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

This tutorial is one of four in a series that demonstrates how to onboard and publish a [sample virtual server image with Terraform](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/tree/v1.0){: external} to {{site.data.keyword.cloud}}. As you complete the tutorial, adapt each step to fit your product's needs.

## Before you begin
{: #vsimage-onboard-prereqs}

1. Create an instance of [{{site.data.keyword.cloud_notm}} Object Storage](/docs/cloud-object-storage?topic=cloud-object-storage-getting-started-cloud-object-storage) and upload your image to a bucket.
2. Create your [VPC](/docs/vpc?topic=vpc-getting-started). 
3. [Import your custom image to all regions](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/tree/main#import-your-custom-image-to-all-supported-regions){: external} in which you want your software to be available. 
4. Create your [Terraform template](/docs/schematics?topic=schematics-create-tf-config). 
5. [Upload your Terraform template and readme file to your GitHub repository](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/tree/main#upload-your-terraform-template-to-a-github-release){: external}. 

  Use the [latest release of the sample Terraform code](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/releases/tag/v1.0 ){: external} as an example of how to set up your repository.
  {: tip}
   
6. Make sure you're assigned the {{site.data.keyword.cloud_notm}} Identity and Access Management (IAM) editor role on the catalog management service and product lifecycle service. See [Assigning access to account management services](/docs/account?topic=account-account-services) for more information.
7. Complete the previous tutorials in the series: [Registering a virtual server image in the Partner Center](/docs/third-party?topic=third-party-vsimage-register) and [Defining the product details of a virtual server image](/docs/third-party?topic=third-party-vsimage-define). 

This tutorial includes deploying the virtual server image to a target VPC. As a result, you will incur associated {{site.data.keyword.cloud_notm}} infrastructure charges. 
{: note}

## Import the virtual server image to your private catalog
{: #vsimage-onboard-import}
{: step}

Complete the following steps to import your virtual server image from your GitHub repository to a private catalog, which was created for you when you registered the virtual server image in {{site.data.keyword.cloud_notm}} Partner Center.

1. Go to the [Partner Center](https://cloud.ibm.com/partner-center/sell){: external} in the {{site.data.keyword.cloud_notm}} console, and click **My products**. 
1. Select your product. 
1. From the Software tab, click **Import a version**.
1. Confirm that **Public repository** is selected as the repository type.
1. Click **Virtual server image with Terraform** to populate the **Source URL** field.

  Alternatively, you can copy and paste `https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample/releases/download/v1.0/isv-vsi-product-deploy-sample.tar.gz` in the field.  

1. Enter `1.0.0` as the software version. 
1. Click **Add version**.
1. Click the name of your product. 
1. Click the **Edit** icon ![Edit icon](../icons/edit-tagging.svg "Edit"). 
1. Select **This Terraform template contains at least one virtual server image.**
1. Click **Save**.

## Configure the deployment values
{: #vsimage-onboard-cfgdeploy}
{: step}

After you import the virtual server image to your private catalog, you're ready to configure the deployment values.

1. From the details page for the virtual server image, click **1.0.0** in the Version list table to navigate to the Configure product tab. 
1. Scroll to the Configure the deployment details section, and click **Add deployment values**. 
1. Select the **Parameter** checkbox to select all options, and click **Add deployment values**.
1. Customize which parameters are required for users to specify during the installation and which ones are hidden from users altogether. For the purposes of this tutorial, configure each parameter as described in the following table.

| Parameter | Description | Required for users to specify? | Hidden from users? |
| --- | ---------- | --- | --- | 
| **`TF_VERSION`** | The version of the Terraform engine that's used in the Schematics workspace. | False | True |
| **`region`** | The region in which the Virtual Private Cloud (VPC) instance is located. | True | False |
| **`ssh_key_name`** | The name of the public SSH key to use when creating the virtual server instance. | True | False |
| **`subnet_id`** | The ID of the subnet within the VPC that the virtual server instance uses. | True | False |
| **`vsi_instance_name`** | The name of the virtual server instance. | True | False |
| **`vsi_profile`** | The profile of the compute CPU and memory resources to use when creating the virtual server instance. | True | False |
| **`vsi_security_group`** | The name of the security group that is created. | True | False |
{: caption="Table 1. Deployment values for a virtual server image" caption-side="top"} 

<br><br>

Next, update the configuration type of the **`region`** parameter:

1. From the Deployment values table, click the **Actions** icon ![Actions icon](../icons/actions-icon-vertical.svg "Actions"), and select **Edit**.
1. Click **Update** next to the `This configuration value is type string` text.
1. Select **VPC region** from the **Configuration type** list, and click **Update**.
1. Click **Update** to save your changes. 

## Add your license agreements
{: #vsimage-onboard-eula}
{: step}

If users are required to accept any license agreements beyond the {{site.data.keyword.cloud_notm}} Services Agreement, provide the details of each agreement.

1. Click **Add license agreements**.
1. Enter the name and URL of the end user license agreement.
1. Click **Update** to save your changes.

## Review your readme file 
{: #vsimage-onboard-readme}
{: step}

The TGZ file that you imported to your private catalog includes a readme file that provides instructions for installing the virtual server image. If you want to make updates to the readme file, you can edit it directly from your private catalog. For the purposes of this tutorial, the following steps describe how to edit the description of the readme file.

1. Click **Edit readme**.
1. Click the **Edit** icon ![Edit icon](../icons/edit-tagging.svg "Edit"), and update the description with the following sentence:

  `Create and deploy a virtual server with ease by using a custom image.`

1. Click **Update** to save your changes. 

## Validate the virtual server image 
{: #vsimage-onboard-validate}
{: step}

Validate that you can deploy the virtual server image to your VPC. 

1. Click **Validate product**.
1. Enter the name of your Schematics workspace, select a resource group, and click **Next**. 
1. In the End user license agreements section, select **I have read and agree to the following license agreements**.
1. Click **Validate**.

  You can monitor the progress of the validation process by clicking **View logs**.
  {: tip}

## Next steps
{: #vsimage-onboard-next}

The virtual server image isn't yet publicly available to other accounts. Use a REST API to make the image public so that users can use it to create virtual server instances. For more information, see [Update the visibility of your image](https://github.com/IBM-Cloud/isv-vsi-product-deploy-sample#update-the-visibility-of-your-image-patch-api){: external}.

After you make the virtual server image public, you can return to the Partner Center and publish it to the catalog. For more information, see [Publishing a virtual server image to the {{site.data.keyword.cloud_notm}} catalog](/docs/third-party?topic=third-party-vsimage-publish).

