---


copyright:
  years: 2020
lastupdated: "2020-10-12"

keywords: software, third-party software, product portal, partner portal, sellers, partners, prerequisites, validate, test, containerized apps, virtual machine, VM, images, partner center

subcollection: third-party

---

{:shortdesc: .shortdesc}
{:external: target="_blank" .external}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:beta: .beta}
{:important: .important}
{:download: .download}

# Validating your software
{: #sw-validate}

The process to validate software includes adding it to a test environment and configuring the version, deployment target, and other details. By validating your software, you're confirming it's ready to be published in the {{site.data.keyword.cloud}} catalog. 
{: shortdesc}

The process to sell third-party software is currently experimental and available solely for vendors that understand the onboarding process is still under development. With the current release, you have the option to bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kala.nenkova@ibm.com.
{: note}

## Before you begin
{: #sw-validate-prereqs}

Make sure you're assigned the editor role on the catalog management service. See [Assigning access to account management services](/docs/account?topic=account-account-services).

Set up the test environment that was previously created for you:

* Install the {{site.data.keyword.cloud_notm}} CLI and the {{site.data.keyword.cloud_notm}} Schematics plug-in. See [Setting up the CLI](/docs/schematics?topic=schematics-setup-cli).
* Upload a readme file that contains your product installation instructions to your GitHub repository. See [Providing your readme file](/docs/third-party?topic=third-party-sw-provide-readme). 
* For containerized apps:
  * Create your [Kubernetes cluster](/docs/containers?topic=containers-getting-started) or [Red Hat OpenShift cluster](/docs/openshift?topic=openshift-getting-started). 
  * For deployments to {{site.data.keyword.cloud_notm}} Kubernetes Service, [set up your Helm chart](/docs/containers?topic=containers-helm). 
  * For deployments to Red Hat OpenShift, set up your [Helm chart](/docs/openshift?topic=openshift-helm) or [operator](/docs/openshift?topic=openshift-operators).
* For virtual machine images:
  * Review the list of [supported images](/docs/vpc?topic=vpc-about-images). 
  * Create your [Terraform template](/docs/schematics?topic=schematics-getting-started).
  * Create an instance of [{{site.data.keyword.cloud_notm}} Object Storage](/docs/cloud-object-storage?topic=cloud-object-storage-getting-started-cloud-object-storage) and add your image to a bucket.

## Adding software to your test environment
{: #sw-validate-add}

Complete the following steps to add your software to the test environment that was previously created for you: 

1. Go to the [{{site.data.keyword.cloud_notm}} console](https://cloud.ibm.com/partner-center/sell/){: external}, and select **Sell** > **Products**.
2. Click the name of your product from the list.
3. Click **Products** > **Private catalog**.
4. Click **Private products** > **Add**.
5. Select whether you are adding your product from a private or public repository. 
6. Enter your repository's URL or TGZ archive. 
7. If you're adding your product from a private repository, you can choose to provide a personal access token or you can use a secret. Instead of giving users a personal access token, you can give them access to a secret and add the token to a secret and centrally manage all tokens and access the secret allows.

  * If you're using a personal access token, select **No** to indicate you aren't using a secret and provide your personal access token.
  * If you're using a secret, select **Yes** and click **Select from Secrets Manager**. Select your service instance, secret group, and secret. If you don't see your secret, make sure you're using the correct secret group and service instance. 
    
    `No service instance available` might be displayed if you haven't created a secret or if you don't have the correct access to use secrets, even if you have service instances that are created. 
    {: note}

8. Select a category and your deployment target.
9. Click **Add**. 

## Editing the configuration details
{: #sw-validate-edits}

Complete the following steps to edit the configuration details for your software:

1. From the Configure product tab, review the version details and prerequisites and constraints.
2. Configure the preinstallation by setting required access and adding the preinstallation instructions and script.
3. Set the deployment values by clicking **Add deployment values**, selecting one or more values from the list, and clicking **Add deployment values**.
4. Optional: Customize your deployment values:

  1. From the **Deployment values** table, click the **Actions** icon ![Actions icon](../icons/actions-icon-vertical.svg) next to the value, and select **Edit**. 
  2. Click **Update** to update the configuration type.
  3. From the **Configuration type** list, select a custom type.
  4. Click **Update**. 
5. From the Add license tab, select a license provider from the list, and click **Add license** to enter the name and URL for your product's license.
6. From the Edit readme tab, the **Edit** icon ![Edit icon](../icons/icon_write.svg) to edit the installation instructions or make updates to the Readme tab that's displayed on your product's catalog details page.
7. From the Validate product tab, configure your validation target. 
8. Click **Update**.
9. Confirm your updates, and click **Validate**. 

After your product is successfully validated, it's displayed in the **Versions** table in the [Partner Center](https://cloud.ibm.com/partner-center/sell/){: external}.
















