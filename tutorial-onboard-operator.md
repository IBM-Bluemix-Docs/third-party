---

copyright:
  years: 2021
lastupdated: "2021-07-07"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, operator, validate, test, Red Hat OpenShift cluster, sample Node-RED Operator, CSV file, CSV, operator bundle

subcollection: third-party

content-type: tutorial
services: Registry
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
{:important: .important}
{:external: target="_blank" .external}
{:step: data-tutorial-type='step'} 


# Onboarding your Operator
{: #operator-onboard}
{: toc-content-type="tutorial"} 
{: toc-services="Registry"}
{: toc-completion-time="45m"} 

This tutorial walks you through how to onboard a sample Node-RED Operator to your private catalog in {{site.data.keyword.cloud}}. By completing this tutorial, you learn how to import the ClusterServiceVersion (CSV) YAML file, configure the deployment, license, and other details, and validate that the Operator can be installed on a Red Hat Openshift cluster.
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

## Before you begin
{: #operator-onboard-prereqs}

1. [Upload your Operator and application images to {{site.data.keyword.registrylong}}](/docs/Registry?topic=Registry-getting-started).
1. [Create your Red Hat OpenShift cluster](/docs/openshift?topic=openshift-getting-started). 
1. Upload your source code to your GitHub repository. 

  Use the [latest release of the sample Node-RED Operator](https://github.com/IBM-Cloud/isv-operator-product-deploy-sample/releases){: external} as an example of how to set up your directory structure. 
  {: tip} 
  
1. Make sure you're assigned the {{site.data.keyword.cloud_notm}} Identity and Access Management (IAM) editor role on the catalog management service and product lifecycle service. See [Assigning access to account management services](/docs/account?topic=account-account-services) for more information.

## Import your CSV file
{: #operator-onboard-import}
{: step}

1. Go to the [Partner Center](https://cloud.ibm.com/partner-center/sell){: external} in the {{site.data.keyword.cloud_notm}} console, and click **My products**.
1. Select the product that you're onboarding.
1. From the Software tab, click **Import a version**.
1. Select **Operator from GitHub repository** as your deployment method.
1. Confirm that **Public repository** is set as the repository type.
1. Enter `https://github.com/IBM-Cloud/isv-operator-product-deploy-sample/blob/main/bundle/1.0.0/manifests/node-red-operator.v1.0.0.clusterserviceversion.yaml` as your source URL. 
1. Enter the software version in the format of major version, minor version, and revision, for example, `1.0.0`.
1. Click **Add product**.

## Set an image pull secret
{: #operator-image-pull-secret}
{: step}

When you create your {{site.data.keyword.openshiftlong}} cluster, the cluster includes an IAM service ID that is given reader access to {{site.data.keyword.registrylong_notm}}. The service ID credentials are authenticated in a non-expiring service ID API key that is stored in image pull secrets in your cluster. As part of configuring the deployment details, you set a pull secret that's used to access and pull your images from the private {{site.data.keyword.registrylong_notm}} respository. 

1. In the Version list table, click the row that contains your Operator.
1. In the Set an image pull secret section, click **Add image pull secret**.
1. Click **Add image pull secret**.
1. Enter the name and value of the image pull secret. 
1. Click **Update**.
1. From the **Image pull secret name** list, select the image pull secret that you just added. 
1. Click **Update**.

## Set the license requirements
{: #operator-onboard-cfg-license}
{: step}

If users are required to accept any license agreements beyond the {{site.data.keyword.cloud_notm}} Services Agreement, provide the URL to each agreement. Or, if users can bring their own licenses, you can provide that URL as well.  

1. Click **Add license agreements** > **Add**. 
2. Enter the name and URL, and click **Update**.

## Review your readme file 
{: #operator-onboard-review-readme}
{: step}

When users access your Operator from the catalog, they can view installation instructions from the Readme tab of your product's catalog details page. The readme information is automatically generated from the details in your CSV file. 

1. Click **Edit readme**.
2. Preview how the information in the readme file will be displayed to users when they are installing the Operator.
3. If you need to make changes, edit the information in the CSV file and import the updated CSV file to your private catalog. 

## Validate the Operator
{: #operator-onboard-validate}
{: step}

1. Click **Validate product**.
1. Select the target cluster and project, and click **Next**.
1. Enter the name of your Schematics workspace, select a resource group, and click **Next**. 

  In the **Tags** field, you can enter a name of a specific tag to attach to your Operator. Tags provide a way to organize, track usage costs, and manage access to the resources in your account.
  {: tip}
  
1. Click **Validate**.

## Next steps
{: #operator-onboard-next}

Return to the Partner Center and submit your request to publish your Operator to the {{site.data.keyword.cloud_notm}} catalog.


