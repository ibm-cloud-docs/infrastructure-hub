---

copyright:
  years: 2024, 2025
lastupdated: "2025-10-30"

subcollection: infrastructure-hub

content-type: faq

---

{{site.data.keyword.attribute-definition-list}}

# FAQ about Microsoft and {{site.data.keyword.cloud}} infrastructure
{: #faqs-for-microsoft-software-ibm-cloud}

IBM is a Gold Certified member of the Microsoft Partner Network&reg; and licensed to sell Microsoft&reg; software under the Services Provider License Agreement (SPLA). IBM is also an authorized license mobility Microsoft partner. Use of Microsoft software is solely subject to terms and conditions from Microsoft. When you use Microsoft software in {{site.data.keyword.cloud_notm}}, you are fully responsible for complying with Microsoft licensing terms.

## What is the relationship between Microsoft and {{site.data.keyword.cloud_notm}}?
{: #faq-microsoft-ibm-cloud}
{: faq}

{{site.data.keyword.cloud_notm}} has a strategic relationship with Microsoft to offer their suite of software. {{site.data.keyword.cloud_notm}} offers native Microsoft software in its offerings. {{site.data.keyword.cloud_notm}} also supports Bring Your Own Licenses (BYOL) for most Microsoft software.

## What types of Microsoft software are supported in {{site.data.keyword.cloud_notm}}?
{: #faq-microsoft-supported-software-ibm-cloud}
{: faq}

You can run most of the Microsoft software on {{site.data.keyword.cloud_notm}} such as

* Windows Server
* SQL Server
* Exchange
* SharePoint
* System Center

You can also use Remote Desktop Services that include some user-specific options such as

* Microsoft Office
* Skype
* Dynamics 365 products

## What support can I expect from {{site.data.keyword.cloud_notm}} for Microsoft products?
{: #faq-microsoft-support-ibm-cloud}
{: faq}

For Microsoft software that is purchased natively on {{site.data.keyword.cloud_notm}}, {{site.data.keyword.cloud_notm}} [support](/docs/account?topic=account-gettinghelp) is the first point of contact for any issue with a Microsoft software-related issue.

IBM provides a choice of support plans.

* Basic
* Advanced
* Premium

For more information, see [IBM support plans](/docs/account?topic=account-support-plans).

## How does {{site.data.keyword.cloud_notm}} and Microsoft work together to solve issues?
{: #faq-microsoft-support-ibm-cloud-solve}
{: faq}

If Microsoft involvement is required to solve a potential issue, {{site.data.keyword.cloud_notm}} [support](/docs/account?topic=account-gettinghelp) engages Microsoft support.

For client BYOL Microsoft software issues, you need to contact [Microsoft support](https://support.microsoft.com/en-us){: external}.

## Does {{site.data.keyword.cloud_notm}} support Extended Security Updates on Microsoft Products ?
{: #faq-extended-support-microsoft-ibm-cloud}
{: faq}

{{site.data.keyword.cloud_notm}} adheres to Microsoft End of Service (EOS) dates. If you purchase extended support updates from Microsoft, you can apply the same dates to your EOS Windows virtual servers. For an OS that is under ESU, contact Microsoft for any issues that are related to the image. For issues that are related to infrastructure or any {{site.data.keyword.cloud_notm}} service, contact [support](/docs/vpc?topic=vpc-getting-help-and-support-for-vpc).

## What support can I expect from {{site.data.keyword.cloud_notm}} for the infrastructure image that I select?
{: #faq-microsoft-ibm-cloud-responsibilities}
{: faq}

{{site.data.keyword.cloud_notm}} provides the cloud infrastructure and Microsoft stock images. {{site.data.keyword.cloud_notm}} [support](/docs/account?topic=account-gettinghelp) covers any issue with the cloud infrastructure and the stock images, such as driver mismatch or licensing. For custom images, the client is responsible for any issues that are related to the custom image, such as a driver mismatch or licensing.

## Is the cost of the Microsoft operating system included in the on-demand {{site.data.keyword.cloud_notm}} virtual server cost?
{: #faq-microsoft-os-cost-ibm-cloud}
{: faq}

For IBM stock images, the operating systems license cost is included as part of the virtual server cost that you see in the catalog.

## Does {{site.data.keyword.cloud_notm}} support Bring Your Own License (BYOL) for Microsoft software?
{: #faq-microsoft-ibm-cloud-byol}
{: faq}

Yes. {{site.data.keyword.cloud_notm}} supports BYOL.

In 2019, Microsoft implemented licensing rules that customers must follow when they use Microsoft licenses on non-Microsoft cloud providers. On 29 August 2022, Microsoft changed their policy. The policy change [announcement](https://www.microsoft.com/en-us/licensing/news/options-for-hosted-cloud){: external} says that you can now deploy a Microsoft BYOL on shared (multi-tenant) hosts. Previously, this rule was limited to dedicated (single-tenant) hosts. Make sure that you read and understand the most recent [Microsoft terms and condition](https://www.microsoft.com/en-us/licensing/news/new-software-assurance-benefit-to-support-hosting-from-third-party-providers){: external}.

A Microsoft [blog post](https://partner.microsoft.com/en-US/blog/article/new-licensing-benefits-make-bringing-workloads-and-licenses-to-partners-clouds-easier/){: external} about BYOL provides more information. Microsoft also provides a [training video](https://licensingschool.eventbuilder.com/hostingcustomer){: external}. When a customer uses BYOL, they can license Windows Server with virtual servers and public multi-tenant virtual servers instead of physical servers.

## Am I charged for BYOL?
{: #faq-microsoft-ibm-cloud-charges-byol}
{: faq}

If you use the BYOL option, you are charged by IBM for only the {{site.data.keyword.cloud_notm}} infrastructure.

## Does a software assurance agreement exist between {{site.data.keyword.cloud_notm}} and Microsoft?
{: #faq-microsoft-ibm-cloud-software-assurance}
{: faq}

License mobility through Microsoft Software Assurance gives Microsoft Volume Licensing customers the flexibility to deploy certain server applications with active Software Assurance on-premises or in the cloud, without having to buy extra licenses. As a result, customers can take advantage of the lowest and flexible cost infrastructure for changing business priorities. Because of this new Software Assurance benefit, customers do not need to purchase new Microsoft Client Access Licenses (CALs) and no associated mobility fees exist.

## What Microsoft products are eligible for license mobility through Software Assurance?
{: #faq-microsoft-products-license-mobility-sa}
{: faq}

The following applications are eligible with Software Assurance.

* Microsoft SQL Server database software
* Microsoft Exchange Server
* Microsoft SharePoint Server
* Microsoft Skype for Business Server
* Microsoft System Center servers
* Microsoft Dynamics 365 Server for Customer Service and Sales applications.

## What is the EOS policy for Microsoft products in {{site.data.keyword.cloud_notm}}?
{: #faq-microsoft-ibm-cloud-eos}
{: faq}

In the lifecycle of an operating system, EOS is the last date that {{site.data.keyword.cloud_notm}} delivers support for a version of a product. {{site.data.keyword.cloud_notm}} [VPC EOS dates](/docs/vpc?topic=vpc-guest-os-lifecycle) and [Classic EOS dates](/docs/bare-metal?topic=bare-metal-product-lifecycle-classic) align with Microsoft EOS dates.

## Can I provision virtual servers in {{site.data.keyword.cloud_notm}} by using EOS software?
{: #faq-microsoft-ibm-cloud-provision-eos}
{: faq}

Yes, you can provision a virtual server by using the EOS OS if it is made into an image template before the EOS date. After you create image template, you can use it to provision servers after the EOS. For more information about creating image templates, see [Creating an image template](/docs/image-templates?topic=image-templates-creating-an-image-template).

## Where can I find the EOS date for Microsoft Servers that run in {{site.data.keyword.cloud_notm}}?
{: #faq-microsoft-eos-dates-ibm-cloud}
{: faq}

For more information about EOS dates for Microsoft software, see [VPC Lifecycle for guest operating systems - Windows Server](/docs/vpc?topic=vpc-guest-os-lifecycle#windows-server) and [Classic Lifecycle for operating systems and add-ons](/docs/bare-metal?topic=bare-metal-product-lifecycle-classic).

## What if a customer wants to keep operating EOS software?
{: #faq-microsoft-ibm-cloud-using-eos}
{: faq}

If the virtual server is provisioned before the EOS date, customer can continue to use EOS software at their own risk while no bug and security fixes are available.
