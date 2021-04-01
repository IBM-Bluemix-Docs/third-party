---


copyright:
  years: 2020, 2021
lastupdated: "2021-04-01"

keywords: software, third-party software, sellers, partners, validate, test, containerized apps, virtual machine, VM, images, partner center

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
{:go: .ph data-hd-programlang='go'}
{:javascript: .ph data-hd-programlang='javascript'}
{:java: .ph data-hd-programlang='java'}
{:python: .ph data-hd-programlang='python'}
{:ui: .ph data-hd-interface='ui'}
{:cli: .ph data-hd-interface='cli'}
{:api: .ph data-hd-interface='api'}

# Onboarding your software
{: #sw-validate}

The process to onboard your software includes importing a version to your private catalog, configuring the deployment details, setting any license requirements, and validating that the version can be successfully installed on the target infrastructure that you require. 
{: shortdesc}

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

## Before you begin
{: #sw-validate-prereqs}

1. Upload your soure code to a release in your GitHub repository. See [Setting up your source code repository](https://docs.github.com/en/github/administering-a-repository/managing-releases-in-a-repository). 
2. Verify that you're using a Pay-As-You-Go or Subscription account. See [Viewing your account type](/docs/account?topic=account-account_settings#view-acct-type) for more information.
3. Make sure you're assigned the editor role on the catalog management service. See [Assigning access to account management services](/docs/account?topic=account-account-services).
4. Set up the test environment that was previously created for you:
  
  * Install the {{site.data.keyword.cloud_notm}} CLI and the {{site.data.keyword.cloud_notm}} Schematics plug-in. See [Setting up the CLI](/docs/schematics?topic=schematics-setup-cli).
  * Upload a readme file that contains your product installation instructions to your GitHub repository. See [Setting up your source code repository](docs/third-party?topic=third-party-source-repo-setup). 
  * For containerized apps:
    * Create your [Kubernetes cluster](/docs/containers?topic=containers-getting-started) or [Red Hat OpenShift cluster](/docs/openshift?topic=openshift-getting-started). 
    * For deployments to {{site.data.keyword.cloud_notm}} Kubernetes Service, [set up your Helm chart](/docs/containers?topic=containers-helm). 
    * For deployments to Red Hat OpenShift, set up your [Helm chart](/docs/openshift?topic=openshift-helm) or [operator](/docs/openshift?topic=openshift-operators).
  * For virtual machine images:
    * Review the list of [supported images](/docs/vpc?topic=vpc-about-images). 
    * Create your [Terraform template](/docs/schematics?topic=schematics-getting-started).
    * Create an instance of [{{site.data.keyword.cloud_notm}} Object Storage](/docs/cloud-object-storage?topic=cloud-object-storage-getting-started-cloud-object-storage) and add your image to a bucket.

## Importing a version to your private catalog
{: #sw-validate-add}

Complete the following steps to import a version of your software to your private catalog. Your private catalog was created for you as part of [Getting set up to sell software](/docs/third-party?topic=third-party-sw-getting-started). 

1. In the {{site.data.keyword.cloud_notm}} console], click the Menu icon ![Menu icon](../icons/icon_hamburger.svg) > **Partner Center > Sell > My Products**. 
2. Select the product that you're onboarding, and click **Software**.
3. Click **Import a version**.
4. Click  **Import a version**.
5. Select whether you are adding your product from a private or public repository. 
6. Enter your repository's URL or TGZ archive. 

  If you're importing a version from a public repository, you can review the following list of supported formats per software type:

  * Node-RED Operator: `https://github.com/IBM-Cloud/isv-operator-product-deploy-sample/blob/main/bundle/1.0.0/manifests/node-red-operator.v1.0.0.clusterserviceversion.yaml`
  * OVA image: `https://github.com/goanalog/OVA-easy/blob/master/metadata.yaml`
  * Terraform template: `https://github.com/Cloud-Schematics/2-zone-vpc/releases/download/v1.0.9/terraform-2-zone-vpc-1.0.9.tgz`
  * Helm chart: `https://charts.bitnami.com/ibm/nginx-8.5.5.tgz`
  
  If you're adding your product from a private repository, you can choose to provide a personal access token or you can use a secret. Instead of giving users a personal access token, you can give them access to a secret, add the token to a secret, and centrally manage all tokens and access the secret allows.

  * If you're using a personal access token, select **No** to indicate that you aren't using a secret and provide your personal access token.
  * If you're using a secret, select **Yes** and click **Select from Secrets Manager**. Select your service instance, secret group, and secret. If you don't see your secret, make sure you're using the correct secret group and service instance. 
    
    The message `No service instance available` might be displayed if you haven't created a secret or if you don't have the correct access to use secrets, even if you have service instances that are created. 
    {: note}

7. Select a category and your deployment target.
8. Click **Add version**. 

## Configuring the product details
{: #sw-validate-cfg-deploy}

The product details will vary based on the type of software that you're onboarding. 

1. From the Configure product tab, review the version details and any prerequisites and contraints. In addition, set the deployment values if applicable. 
1. Set the applicable deployment values if applicable.
1. Click **Update** to save your changes. 

## Adding license details
{: #sw-validate-add-license}

If users are required to accept any license agreements beyond the IBM Cloud Services Agreement, provide the URL to each agreement. Or, if users can bring their own licenses, you can provide that URL as well.

1. Click **Add license** > **Add**. 
2. Enter the name and URL, and click **Update**.

## Reviewing your readme file
{: #sw-validate-readme-review}

When users access your software from the catalog, they can view installation instructions from the Readme tab of your product's catalog details page. The information on the Readme tab is generated from the readme file that you uploaded to your GitHub repository. 

1. Click **Edit readme**.
2. Preview how the information in the readme file will be displayed to users when they are installing the software.
3. If you need to make changes, click the Edit icon ![Edit icon](../icons/edit-tagging.svg) next to the Readme section title.
4. Click **Update** to save your changes.

## Configuring the validation target 

1. From the Validate product tab, configure your validation target. 
1. Click **Update**.
1. Confirm your updates, and click **Validate**. 

After the software version is successfully onboarded, it's displayed in the Versions table in the [Partner Center](https://cloud.ibm.com/partner-center/sell/){: external}.





















