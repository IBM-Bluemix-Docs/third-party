---

copyright:
  years: 2020
lastupdated: "2020-12-16"

keywords: troubleshoot software, Helm, helm chart, repo, HTTPS protocol

subcollection: third-party

content-type: troubleshoot

---

{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:troubleshoot: data-hd-content-type='troubleshoot'}

# Why can't I upload my Helm chart repository?
{: #repo-upload-error}
{: troubleshoot}

You receive the following error message when you try to upload your Helm chart repository:
{: tsSymptoms}

`There was an error while contacting this URL.`

This error typically occurs because the repository doesn't support HTTPS protocol. 
{: tsCauses}

Make sure your repository supports HTTPS protocol. 
{: tsResolve}
