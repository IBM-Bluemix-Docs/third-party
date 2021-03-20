---

copyright:

  years: 2020, 2021

lastupdated: "2021-03-19"

keywords: end-to-end, software onboarding, checklist, third party, product portal, requirements, sellers, partner portal, partners, third-party software

subcollection: third-party

---

{:right: .ph data-hd-position='right'}
{:shortdesc: .shortdesc}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:beta: .beta}
{:term: .term}
{:external: target="_blank" .external}


# Checklist for selling software on {{site.data.keyword.cloud_notm}}
{: #checklist-software}

Use the following checklist to track all the tasks that are required to successfully sell your third-party software on {{site.data.keyword.cloud}}.
{:shortdesc}

The process to sell third-party software is available solely for providers that understand the onboarding process is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kala.nenkova@ibm.com.
{: beta}

## Complete the getting started tasks
{: #sw-start-checklist}

The following tasks are typically completed by a team member who is familiar with the business case and other members of the team who might help with the onboarding process. 

| Task | Description | Environment |
|------|-------------|-------------|
| ☐ Provide company and product details | Specify the names of your company and product.  | {{site.data.keyword.cloud_notm}} console | 
| ☐ Review and sign the {{site.data.keyword.IBM}} Digital Provider Agreement | Indicate that you understand the terms and signed the agreement between you and {{site.data.keyword.IBM_notm}}. | {{site.data.keyword.cloud_notm}} console |
| ☐ Create a test environment | The test environment is used to validate the readiness of your software. | {{site.data.keyword.cloud_notm}} console |
| ☐ Assign team access | With the correct access assigned, members of your team can help onboard your software. | {{site.data.keyword.cloud_notm}} console |
{: caption="Table 1. Getting started tasks for selling software" caption-side="top"} 

For more information about each task, see [Getting started with software](/docs/third-party?topic=third-party-sw-getting-started). 

## Define your software details 
{: #sw-details-checklist}

The following tasks are typically completed by a team member familiar with the business case, marketing details, and customer support experience for the product. 

| Task | Description | Environment |
|------|-------------|-------------|
| ☐ Verify your company and product information | Review the details that you provided as part of the getting started tasks to make sure that everything is correct. | {{site.data.keyword.cloud_notm}} console |
| ☐ Provide your Cloud Resource Name (CRN) | The CRN is necessary for identifying a specific resource unambiguously across all products in {{site.data.keyword.cloud_notm}}. | {{site.data.keyword.cloud_notm}} console |
| ☐ Develop your catalog entry | Add your product logo, description, and other details for your software's entry in the {{site.data.keyword.cloud}} catalog. | {{site.data.keyword.cloud_notm}} console |
| ☐ Define your customer support experience | Provide details about how users can get help with using your software.  | {{site.data.keyword.cloud_notm}} console |
{: caption="Table 2. Tasks for defining software details" caption-side="top"} 

For more information about each task, see [Defining your software details](/docs/third-party?topic=third-party-sw-product-details).

## Validate your software
{: #sw-validate-checklist}

The following tasks are typically completed by a technical member of your team.

| Task | Description | Environment |
|------|-------------|-------------|
| ☐ Create your readme file | The readme file describes how users can install your software and get customer support. | Your GitHub repository |
| ☐ Complete the prerequisites | Confirm you have the correct level of IAM access. Install the {{site.data.keyword.cloud_notm}} CLI and the {{site.data.keyword.bpshort}} CLI plug-in. Complete other prerequisites that are required for certain types of software. | {{site.data.keyword.cloud_notm}} console, GitHub, and your test environment |
| ☐ Configure your software | Set the version, preinstallation details, deployment target, and license requirements. | {{site.data.keyword.cloud_notm}} console |
| ☐ Validate your software | Validate that your software is ready to be delivered to the public catalog. | {{site.data.keyword.cloud_notm}} console |
{: caption="Table 3. Tasks for validating software" caption-side="top"} 

For more information about each task, see the following links:

* [Creating your readme file](/docs/third-party?topic=third-party-sw-provide-readme)
* [Validating your software](/docs/third-party?topic=third-party-sw-validate)

