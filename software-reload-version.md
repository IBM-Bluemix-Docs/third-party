---


copyright:
  years: 2021
lastupdated: "2021-07-06"

keywords: software, third-party software, sellers, partners, versions, test, partner center, reload 

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


# Reload a version of your software
{: #software-reload}

You can reload a version of your software in your private catalog to update the version based on your current repository. This feature can be used to revert your version to its default state when it was first imported.
{: shortdesc}

The process to sell third-party software is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you have questions, contact us at kdmeyer@ibm.com.
{: beta}

## Reload a version that is not published
{: #software-reload-catalog}

To update a version of your software that is not published, you must reload the version from your source repository and validate it.  

1. In the {{site.data.keyword.cloud_notm}} console, select **Manage > Catalogs > Private catalogs**. 
1. Select the private catalog where your product is located. 
1. Select your product. 
1. Select the version of the software you would like to reload. 
1. Open the **Actions** menu and select **Reload version**.
1. Click **Reload version**. 
1. Configure and validate your software. 

Configuration and validation steps vary based on the type of software.
{: note}

## Reload a published version
{: #software-reload-published}

To update a published version of your software, you must create a draft, reload the version from your source repository, validate, and merge the changes.  

1. In the {{site.data.keyword.cloud_notm}} console, select **Manage > Catalogs > Private catalogs**. 
1. Select the private catalog where your product is located. 
1. Select your product. 
1. Select the version of the software you would like to reload. 
1. Open the **Actions** menu and click **Edit** to create a draft of your original version.
1. In the draft version, open the **Actions** menu and click **Reload version**.
1. In the Reload version panel, click **Reload version**. 
1. Configure and validate your software. 

   Configuration and validation steps vary based on the type of software.
   {: note}

9. Open the **Actions** menu and click **Merge changes**.
10. Click **Merge** to update your original version.
