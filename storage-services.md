---

copyright:
  years: 2020, 2026
lastupdated: "2026-09-14"

keywords: IBM Cloud storage services, virtual private cloud storage, block storage, file storage, object storage, scalable storage, data security

subcollection: infrastructure-hub

---

{{site.data.keyword.attribute-definition-list}}

# Choosing {{site.data.keyword.cloud_notm}} storage services for your workloads
{: #storage}

Discover {{site.data.keyword.cloud_notm}} storage services that offer scalable, secure, and cost-effective data storage solutions for traditional and cloud-native workloads.
{: shortdesc}

Choose from block storage, file storage, and object storage options across VPC and classic infrastructure.

## Current infrastructure
{: #storage-vpc}

VPC infrastructure provides the latest generation of cloud-native storage services, offering high performance, zonal redundancy, and integrated security for modern workloads.

| Option | Description |
|--------|---------------|
| [{{site.data.keyword.block_storage_is_short}}](/docs/vpc?topic=vpc-block-storage-about) | Persistent, high-performance data storage for virtual server instances in the {{site.data.keyword.cloud}} Virtual Private Cloud (VPC). The VPC infrastructure provides rapid scaling across multiple regions and zones, and extra performance and security.  |
| [{{site.data.keyword.filestorage_vpc_full}}](/docs/vpc?topic=vpc-file-storage-vpc-about) | A zonal file storage offering that provides NFS-based file storage services. You can create file shares in a zone and share them with virtual server instances across zones and VPCs in the same region. You can also share your NFS-based file storage across accounts and external services, such as [IBM watsonx](https://dataplatform.cloud.ibm.com/docs/content/wsj/getting-started/welcome-main.html?context=wx){: external}. To restrict access to a specific virtual server instance within a VPC, use security groups, and encrypt the data in transit. Compatible with {{site.data.keyword.vsi_is_short}} and {{site.data.keyword.bm_is_short}}. |
| [{{site.data.keyword.cos_full_notm}}](/docs/cloud-object-storage?topic=cloud-object-storage-getting-started-cloud-object-storage) | Distributed, multi-tenant Cloud Object Storage for data encrypted and dispersed across multiple geographic locations, which are accessed over HTTPS by using a REST API. This service uses the distributed storage technologies that are provided by the {{site.data.keyword.cos_full_notm}} System. |
{: caption="Storage options" caption-side="bottom"}

## Classic infrastructure
{: #storage-classic}

Classic infrastructure storage services provide persistent, network-attached options for traditional workloads that require dedicated storage independent of compute resources.

| Option | Description |
|--------|---------------|
| [{{site.data.keyword.blockstorageshort}}](/docs/BlockStorage?topic=BlockStorage-getting-started) | Persistent, high-performance iSCSI storage that is provisioned and managed independently of Compute instances. iSCSI-based {{site.data.keyword.blockstorageshort}} LUNs are connected to authorized devices through redundant multipath I/O (MPIO) connections. |
| [{{site.data.keyword.filestorage_short}}](/docs/FileStorage?topic=FileStorage-getting-started) | Persistent, fast, and flexible network-attached, NFS-based {{site.data.keyword.filestorage_short}}. In this network-attached storage (NAS) environment, you have total control over your file shares function and performance. {{site.data.keyword.filestorage_short}} shares can be connected to up to 64 authorized devices over routed TCP/IP connections for resiliency. For more information, see the [FAQ for {{site.data.keyword.filestorage_short}}](/docs/FileStorage?topic=FileStorage-file-storage-faqs#authlimit). |
| [{{site.data.keyword.backup_full}}](/docs/Backup?topic=Backup-getting-started) | An automated agent-based backup system that is managed through a browser-based management utility. You can back up data between servers in one or more data centers on the {{site.data.keyword.cloud}} network. |
{: caption="Storage options - Classic" caption-side="bottom"}

## Next steps
{: #storage-nextsteps}

To continue, see [Managing your infrastructure](/docs/infrastructure-hub?topic=infrastructure-hub-managing).
