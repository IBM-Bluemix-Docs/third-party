---

copyright:
  years: 2021
lastupdated: "2021-07-06"

keywords: onboard software, third-party software, sell on IBM Cloud, partner center, operator, validate, test, sample Red Hat OpenShift operator, operator bundle

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
{:important: .important}
{:beta: .beta}
{:external: target="_blank" .external}
{:step: data-tutorial-type='step'} 

# Onboarding your Operator bundle from the Red Hat Certified registry
{: #bundle-onboard}
{: toc-content-type="tutorial"} 
{: toc-services="Registry"}
{: toc-completion-time="45m"} 

This tutorial walks you through how to onboard an Operator bundle in {{site.data.keyword.cloud}}. By completing this tutorial, you learn how to import the Red Hat OpenShift Operator bundle, configure the deployment, license, and other details, and validate that the Operator bundle can be installed on a cluster.
{: shortdesc}

This tutorial is one of four in a series that demonstrates how to onboard and publish an Operator bundle. It uses a fictitious company that's called *Example Corp* to onboard the real Akka Cluster Operator from the Red Hat OpenShift Certified registry. As you complete the tutorial, adapt each step to fit your product's needs.

The process to sell third-party software is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you have questions, contact us at kdmeyer@ibm.com.
{: beta}


## Before you begin
{: #bundle-onboard-prereqs}

1. Confirm that your Operator bundle exists in the Red Hat OpenShift Certified registry.
1. [Create your Red Hat OpenShift cluster](/docs/openshift?topic=openshift-getting-started). 
1. [Upload your Operator bundle and application images to {{site.data.keyword.registrylong}}](/docs/Registry?topic=Registry-getting-started).
1. Verify that you're assigned the correct roles. For more information, see [Assigning access to account management services](/docs/account?topic=account-account-services) and [Managing access to resources](/docs/account?topic=account-assign-access-resources).
   * Administrator on all account management services and all IAM services
   * Editor on the catalog management service
   * Editor on the Container Registry service
   * Administrator on the Red Hat OpenShift cluster
   * Editor on the software instance service

Make sure that you use the same account to access the IBM Cloud Registry and to create the Red Hat OpenShift cluster.
{: important}

## Import your Operator bundle
{: #bundle-onboard-import}
{: step}

1. Go to the [Partner Center](https://cloud.ibm.com/partner-center/sell){: external} in the {{site.data.keyword.cloud_notm}} console, and click **My products**. 
1. Select the product that you're onboarding.
1. From the Software tab, click **Import a version**.
1. Choose **Operator from Red Hat registry** as your deployment method. 
1. Select **Certified** as your Red Hat repository. 
1. Select **Akka Cluster Operator** as your Operator.
1. Select the Operator bundle version that you would like to import.  
1. Enter the software version that the Operator bundle installs in the format of major version, minor version, and revision. For example, you can use Operator version `1.1.0` to install software version `3.1.1`. 
1. Review the summary of your Operator bundle. 
1. Click **Add version**.

## Configure your Operator bundle
{: #bundle-configure}
{: step}

From the Configure product tab, you can review your version details. There are no actions that you need to take. 

## Set the license requirements
{: #bundle-onboard-cfg-license}
{: step}

If users are required to accept any license agreements beyond the {{site.data.keyword.cloud_notm}} Services Agreement, provide the URL to each agreement. Or, if users can bring their own licenses, you can provide that URL as well.  

1. From the Add license agreements tab, click **Add**. 
2. Enter the name and URL, and click **Update**.

## Review your readme file 
{: #bundle-onboard-review-readme}
{: step}

When users access your Operator bundle from the catalog, they can view installation instructions from the Readme tab of your product's catalog details page. The readme information is automatically generated. 

1. From the Edit readme tab, click the **Edit** icon![Edit icon](../icons/edit-tagging.svg "Edit").
2. Preview how the information in the readme file will be displayed to users when they are installing the Operator bundle.
3. If you need to make changes, edit the information in the source file and import the updated Operator bundle to your private catalog. 

## Validate the software version
{: #bundle-onboard-validate}
{: step}

Before publishing the Operator bundle, you need to validate it to make sure that the version can be deployed to the intended target. 

1. From the **Validate product** tab, select the Update channel that you would like to receive updates from. 
1. Select whether you would like updates to be applied automatically or manually. 
1. Select a Red Hat OpenShift cluster. 
1. Select a project. 
1. Click **Next**.
1. Confirm or edit your workspace name.  
1. Select a resource group. 
1. Enter tags for your workspace. 
1. Click **Next** 
1. Click **Validate**. 

## Next steps
{: #bundle-onboard-next}

Return to the Partner Center and submit your request to [publish your Operator bundle](/docs/third-party?topic=third-party-bundle-publish) to the {{site.data.keyword.cloud_notm}} catalog.


