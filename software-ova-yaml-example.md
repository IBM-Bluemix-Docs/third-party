---


copyright:
  years: 2020
lastupdated: "2020-10-12"


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

# Example YAML file for onboarding OVA images
{: #3p-ova-prereqs}

The process to onboard OVA images is the same as onboarding other third-party software except you need to add a YAML file that contains required onboarding information. Manually create the YAML and add it to your GitHub repo that you reference during the onboarding process.  
{: shortdesc}

The process to sell third-party software is currently experimental and available solely for vendors that understand the onboarding process is still under development. With the current release, you have the option to bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kala.nenkova@ibm.com.
{: note}

After you complete this prerequisite, you're ready to add your OVA image to the private catalog you're using for onboarding, and validate that it's ready for publishing. See [Validating your software](/docs/third-party?topic=third-party-sw-validate).

## Required metadata
{: #ova-metadata}

The following table lists the metadata to include in your YAML file:

| Metadata key  | Required | Description |
|---------------|----------|-------------|
| `app_id`      | ![Feature available](../icons/icon_enabled.svg) | The programmatic name of the product. Not exposed to the user. |
| `title`       | ![Feature available](../icons/icon_enabled.svg) | The name of the product externally displayed in the public catalog. |
| `version`     | ![Feature available](../icons/icon_enabled.svg) | The version ID of the OVA image. You must update each time that you update the OVA image. This value must be in semantic versioning, for example, `1.0.0`, `1.0.1`, `1.0.2`. | 
| `revision`    | ![Feature available](../icons/icon_enabled.svg) | The version of the OVA Metadata. You must update each time that you update your metadata. |
| `kind`        | ![Feature available](../icons/icon_enabled.svg) | The value is always `ova`. |
| `image`       | ![Feature available](../icons/icon_enabled.svg) | The object that contains `url` or `sha256` values. |
| `url`         | ![Feature available](../icons/icon_enabled.svg) | A child value of `image`. The URL for the `image` path. |
| `sha256`      | ![Feature available](../icons/icon_enabled.svg) | A child value of `image`. The signature of the file referenced in `image`. |
| `eula_url`    |          | The link to publicly accessible license document. |
| `eula_label`  |          | The label for the license link. |
| `categories`  |          | The array of {{site.data.keyword.Bluemix_notm}} Catalog categories to filter items in the catalog. For more information about categories, see [Defining your software details](/docs/third-party?topic=third-party-sw-product-details). |
| `logo`        | ![Feature available](../icons/icon_enabled.svg) | The URL path to the product icon externally displayed in the public catalog along with the `title` value. |
| `description` | ![Feature available](../icons/icon_enabled.svg) | The short description of the OVA image externally displayed in the public catalog along with the `title` and `logo` values. |
| `readme`      | ![Feature available](../icons/icon_enabled.svg) |  The readme file text for this ova image, in markdown format. |
| `links`       |          | Links to support or documentation. Not required. |
{:caption="Table 1. Required metadata for OVA images" caption-side="top"}


## Example

The following example shows a YAML file that is formatted with the required metadata. 

```
app_id: devName
title: productName
version: 5.4.2-0
revision: 3
kind: ova,
image:
 url: https://productURL-5.4.2-0.ova
 sha256: 1aaa22bbb33c44444dd5e66f4g7hh8i99j11kk22ll33m4nn5555o6pp77qq888r
eula_url: https://www.product.org/licenses/LICENSE-2.0.txt
eula_label: Product 2.0
categories:
- network
logo: https://productIcon.net/images.png
description: "Description for OVA image offering."
readme: The full text for the required readme about the ova image.
links:
- id: docs_index
 title: Getting started
 url: https://docs.OVAimage-gettingStarted.com
- id: support_index
 title: Product Support
 url: https://docs.OVAimage-support.com
```



