---


copyright:
  years: 2020
lastupdated: "2020-10-08"

keywords: onboard software, third-party software, sell on IBM Cloud, catalog details, support, software, product portal, provider portal, partner, sellers, partner portal, catalog, CRN, cloud resource name, product lifecycle

subcollection: third-party

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:beta: .beta}
{:important: .important}
{:download: .download}
{:external: target="_blank" .external}

# Defining your software details 
{: #sw-product-details}

Onboarding your software to {{site.data.keyword.cloud}} consists of providing certain details about your product, including a CRN value, a product description and logo, and your customer support details.
{: shortdesc}

The process to sell third-party software is currently experimental and available solely for evaluation and testing purposes. If you’re interested in trying it out, contact us at kala.nenkova@ibm.com.
{: note}

## Before you begin
{: #sw-details-prereqs}

Make sure you're assigned the following Identity and Access Management (IAM) roles:

  * Editor on the IAM access groups service
  * Editor on the catalog management service
  * Editor on the product lifecycle service 

For more information, see [Assigning access to account management services](/docs/account?topic=account-account-services). 

## Defining your CRN 
{: #sw-details-crn}

The value of your Cloud Resource Name (CRN) serves as a customer-facing unique identifier that's used to identify a specific resource unambiguously across all {{site.data.keyword.cloud_notm}} products. Make sure that the value adequately reflects your product. For more details, see [Cloud Resource Names](/docs/account?topic=account-crn).

Complete the following steps to define your CRN:

1. Go to the [{{site.data.keyword.cloud_notm}} console](https://cloud.ibm.com/partner-center/sell/){: external}, and click **Sell** > **Products**. 
2. Select the software version that you want to onboard. 
3. From the Details tab, import the version of your product CRN.

  The CRN value must be immutable and can’t change during the lifecycle of the product that it refers to.
  {: important}

## Defining your catalog entry 
{: #sw-details-catalog}

Your catalog entry includes details that are publicly displayed in the {{site.data.keyword.cloud_notm}} catalog. The details that you're required to provide are intended to help users discover your software in the catalog. Complete the following steps to define your entry and get a preview of how it will be displayed: 

1. Click **Catalog entry**.
2. In the **Company or product logo** field, enter the fully-qualified URL to your company or product logo. Make sure the image is an SVG file sized at 32 x 32 pixels.
3. In the **Description** field, summarize the value of your software in 130 characters or less.
4. Click **Add category** and select one option from the list to set the catalog category in which your software should be listed. See the following list for a description of each category:

  <dl>
  <dt>AI / Machine Learning</dt>
  <dd>Products that enable systems to learn from data rather than through explicit programming.</dd>
  <dt>Analytics</dt>
  <dd>Products that facilitate the analysis of data, typically large sets of business data, by the use of mathematics, statistics, and other means.</dd>
  <dt>Blockchain</dt>
  <dd>Products that facilitate the process of recording transactions and tracking assets in a business network.</dd>
  <dt>Compute</dt>
  <dd>Infrastructure resources that serve as the basis for building apps in the cloud. </dd>
  <dt>Containers</dt>
  <dd>A standard unit of software that packages up code, and all its dependencies, so the app runs quickly and reliably from one computing environment to another. </dd>
  <dt>Databases</dt>
  <dd>Products that provide some form of access to a database without requiring setting up physical hardware, installing software, or configuring for performance.</dd>
  <dt>Developer tools</dt>
  <dd>Products that support developing, testing, and debugging software.</dd>
  <dt>Integration</dt>
  <dd>Products that facilitate the connection of data, apps, APIs, and devices across an organization to be more efficient, productive, and agile.</dd>
  <dt>Internet of Things</dt>
  <dd>Products that support receiving and transferring data over wireless networks without human intervention.</dd>
  <dt>Logging and monitoring</dt>
  <dd>Products that support storing, searching, analyzing, and monitoring log data and events. And, products that support reviewing and managing the operational workflow and processes being logged.</dd>
  <dt>Mobile</dt>
  <dd>Products with specific or special utility for users creatings things to be used on mobile devices.</dd>
  <dt>Networking</dt>
  <dd>Products that support or augment the linking of computers so they can operate interactively.</dd>
  <dt>Security</dt>
  <dd>Products that provide the protection of stored data from theft, leakage, and deletion.</dd>
  <dt>Storage</dt>
  <dd>Products that support data to be created, read, updated, and deleted.</dd>
  </dl>

5. Click **Filters** and select one or more options to set filters that users can use to narrow catalog search results.
6. In the **Keywords** field, enter the keywords that users will most likely use to search for your software in the catalog.

## Defining your customer support experience
{: #sw-details-support}

Making sure your users understand how to get help and support is key. Complete the following steps to define your support experience: 

1. Click **Support**.
2. In the **Support URL** field, enter the fully-qualified URL to your support website, for example, `https://support.examplecorp.com/`.
3. In the **Support response process** field, enter a description of your support response process, for example: 

  `This product is provided and supported by Example Corp. If you encounter problems, you can open a support issue with the Example Corp support team. Responses to support issues are typically provided in approximately 1 to 2 business days.` 

4. In the **Support contacts** field, enter a description of how users can contact support, for example:

  `If you run into issues, you can contact Example Corp by chat at https://support.examplecorp.com/chat or by phone at https://support.examplecorp.com/phone 24 hours a day, 7 days a week.`

5. In the **Support location** field, enter the countries in which support is located, for example:

  `Example Corp support teams are located in the following countries: United States, Japan, India, Ireland.`



