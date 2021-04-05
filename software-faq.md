---

copyright:

  years: 2020, 2021

lastupdated: "2021-04-01"

keywords: third-party software, faq, partners, sellers, help, third-party, software, partner center, frequently asked questions

subcollection: third-party

content-type: faq

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:external: target="_blank" .external}
{:faq: data-hd-content-type="faq"}
{:support: data-reuse='support'}
{:note: .note}
{:beta: .beta}

# FAQs about selling software
{: #thirdparty-sw-faqs}

FAQs about selling third-party software on {{site.data.keyword.cloud}} might include questions about the types of software you can add to the catalog, pricing plans, and updating and restoring software versions. 
{: shortdesc}

To find all FAQs for {{site.data.keyword.cloud_notm}}, see our [FAQ library](/docs/faqs).

The process to sell third-party software is available solely for providers that understand that the onboarding process is still under development. With the current release, you can bring your own licenses or deliver your third-party software for free. If you’re interested in trying it out, contact us at kdmeyer@ibm.com.
{: beta}

## What types of software can I add to the {{site.data.keyword.cloud_notm}} catalog? 
{: #supported-sw}
{: faq}

See the following list for the types of third-party software that you can currently add to the catalog:
   * Helm charts
   * Terraform templates
   * OVA images deployed on VMware vSphere
   * Operators deployed on Red Hat OpenShift

## What account do I use to onboard my software? 
{: #accountuse-sw}
{: faq}

Use your {{site.data.keyword.cloud_notm}} account to onboard software to the catalog. In some cases an {{site.data.keyword.IBM_notm}} representative, with their own account, might be helping you with the onboarding process. If you want the representative to access your software in your test environment, you can add them to your account. For more details, see [Inviting users to an account](/docs/account?topic=account-iamuserinv)

## How do I upload a version from my GitHub repository?
{: #gh-upload-sw}
{: faq}

See [Managing releases in a repository](https://docs.github.com/en/github/administering-a-repository/managing-releases-in-a-repository){: external}.

## How do I view my account ID and type? 
{: #accounttype-sw}
{: faq}

Go to **Manage** > **Account** > **Account settings** in the console. Your account ID is the alphanumeric value in the Account section. Your account type is included in the Account type section. 

## Can I include a pricing plan with my software?
{: #pricing-sw}
{: faq}

Currently, software products in the {{site.data.keyword.cloud_notm}} catalog don't include pricing plans. You can bring your own licenses or deliver your third-party software for free. 

## How do I update my software?
{: #update-versions}
{: faq}

To update your software, you can add a new version of it or update and republish an existing version. For more details, see [Updating your software](/docs/third-party?topic=account-update-private).

Make sure the version of the software that you're updating in your private catalog is the same as the version that was onboarded in the Partner Center UI.  
{: note} 

## Can I restore a deprecated version of software?
{: #update-versions}
{: faq}

Yes. To restore a deprecated version, validate and publish it again. For more details, see [Deprecating and restoring software versions](/docs/third-party?topic=account-dep-restore). 

Make sure the version of the software that you're restoring in your private catalog is the same as the version that was onboarded in the Partner Center UI.
{: note}

## Can I invite a team member to help onboard software?
{: #invite-team}
{: faq}

Yes, you can add team members to help onboard software. You need to assign them specific levels of access. For more information, see [Inviting team members to help onboard software](/docs/third-party?topic=third-party-sw-invite-team).

## Can I remove a team member's access to my account?
{: #remove-team}
{: faq}

Yes, go to **Manage > Access (IAM)** in the console, select **Users**, find the user that you want to remove, select **Remove user** from the **Actions** menu.

Only account owners and users with specific access can remove a user. For more information, see [Removing users from an account](/docs/account?topic=account-remove).

## Can I view my assigned roles and permissions?
{: #access-onboard}
{: faq}

Yes, go to **Manage > Access (IAM)** in the console, and select your name on the **Users** page. Then, depending on the access you're looking for, select the different tabs:

   * To determine what access you have through the access groups you are assigned, select **Access groups**.
   * To see IAM access policies that are assigned to you, select the **Access policies**.

## Can I delete my product from the catalog? 
{: #delete-product}
{: faq}

No, but you can deprecate a software version. When you deprecate a version, users cannot view the product in the catalog nor can they install it. For more information, see [Deprecating and restoring software versions](/docs/third-party?topic=account-dep-restore).

## How long does it take to onboard a product? 
{: #time-onboard}
{: faq}

The complete onboarding process for software takes approximately 7 days. 

## What do I do if my product is not approved? 
{: #approval-denied}
{: faq}

If your product is not approved, you receive feedback in the console. The feedback includes why your product was not approved and what items need to be updated to receive approval. After you update the product, you can resubmit your product for approval.

## Why can't I find the product I'm onboarding? 
{: #missing-products}
{: faq}

If you can't find the product that you are onboarding, first make sure that you are in the correct account. If you are in the correct account and your product is not listed on the My products page, your product was possibly deleted. Unfortunately, if your in-progress product was deleted, you must restart the onboarding process.



