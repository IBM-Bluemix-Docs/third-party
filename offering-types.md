---

copyright:

  years: 2018, 2020

lastupdated: "2020-08-13"

keywords: party offering types, third-party offering, billing service

subcollection: third-party

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:external: target="_blank" .external}

# Third-party product types
{: #offering-types}

You can deliver your third-party product as an integrated billing service or a referral service in {{site.data.keyword.Bluemix}}.
{:shortdesc}

Delivering your third-party product as an integrated billing service means that users can select from different {{site.data.keyword.IBM}} pricing plans that are listed on your catalog details page in the {{site.data.keyword.Bluemix_notm}} console. Additionally, users can automatically create an instance of your third-party product.

When you deliver your third-party product as a referral service, users are directed to your website from the catalog details page in the {{site.data.keyword.Bluemix_notm}} console. From your website, users create accounts and get the appropriate credentials. These credentials are needed to programmatically connect your third-party product to an app they're building on {{site.data.keyword.Bluemix_notm}}.

## Comparing product types
{: #compare}

The following table provides a detailed comparison of the third-party product types.

|  | Integrated Billing Service  | Referral Service |
|---|---|---|
| **Onboarding** | Onboarding is handled through the {{site.data.keyword.IBM_notm}} Provider workbench and the resource management console. The provider develops an Open Service Broker, hosting it, testing it, and publishing their product through a series of self-service steps. | Onboarding is handled through the Provider workbench. The self-service onboarding process takes about two weeks. |
| **Deploying** | Created by the {{site.data.keyword.Bluemix_notm}} platform | API-based services only |
| **Billing**  |  In the integrated billing model, the user receives a single bill for both their {{site.data.keyword.IBM_notm}} product and their integrated third-party product. | In the referral model, providers' bill the user and keep 100% of the revenue.  |
| **Example** | [ElephantSQL](https://{DomainName}/catalog/services/elephantsql){: external} | [Accern API](https://{DomainName}/catalog/services/accern-api){: external} |
{: caption="Table 1. Comparison of third-party product types" caption-side="top"}

