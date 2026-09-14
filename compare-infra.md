---
copyright:
  years: 2019, 2026

lastupdated: "2026-09-14"

keywords: infrastructure as a service, classic infrastructure, VPC infrastructure, infrastructure comparison, IBM Cloud infrastructure environments

subcollection: infrastructure-hub

---

{{site.data.keyword.attribute-definition-list}}

# Comparing classic and VPC infrastructure on {{site.data.keyword.cloud_notm}}
{: #compare-infrastructure}

Compare the key differences between {{site.data.keyword.cloud_notm}} classic and VPC infrastructure environments to choose the best option for your workloads and applications.
{: shortdesc}

If you aren't familiar with the environment types, review the following descriptions. Watch the [Bare Metal Servers: Classic versus VPC Infrastructure Explainer Video](https://mediacenter.ibm.com/media/IBM%20Bare%20Metal%20Servers%20-%20Classic%20vs.%20VPC%20Infrastructure%20Explainer%20Video/1_hn1d69nn){: external} to learn more about the differences between the classic and VPC infrastructures.

* The classic infrastructure is the existing Infrastructure as a Service (IaaS) platform. This environment is best for lift and shift workloads so you can move applications quickly and keep the same architecture.
* VPC infrastructure is the new IaaS platform, based on software-defined networking and ideal for cloud-native applications.

## Key takeaways
{: #compare-key-takeaways}

VPC infrastructure is the recommended platform for new workloads, offering modern cloud-native capabilities across every dimension. Classic infrastructure remains the right choice for lift-and-shift migrations and workloads that depend on its existing architecture. The most significant differences are:

Compute
:   VPC provides more profile families, including AI Optimized, Confidential Compute, and Storage Optimized, along with auto scaling and instance groups that classic infrastructure does not offer.

Network
:   VPC replaces physical and virtual network appliances with built-in cloud-native functions that include VPN-as-a-service, Load Balancer for VPC, and built-in network isolation, simplifying network operations.

Storage
:   Both environments support block and file storage with encryption and snapshots, but VPC adds optional encryption in transit, cross-account key authorization, and cross-account access for file shares.

Security
:   VPC provides built-in security groups and network access control lists (ACLs) without requiring third-party appliances.

API
:   VPC uses a modern REST-based API, replacing the classic SoftLayer API (SLAPI) with a developer-friendly interface aligned with {{site.data.keyword.cloud_notm}} platform standards.

## Compute differentiators
{: #compare-compute}

Classic infrastructure offers customizable bare metal and virtual servers, while VPC infrastructure adds cloud-native capabilities such as auto scaling, instance groups, and profiles optimized for AI and confidential computing.

| Category   |  Classic infrastructure   | VPC infrastructure |
| ---------- | ------------------------- | ------------------ |
|  **Services**  | * {{site.data.keyword.BluVirtServers_short}} \n * {{site.data.keyword.baremetal_short}} \n * Dedicated hosts \n * Reserved virtual servers  | * {{site.data.keyword.BluVirtServers_short}} \n * {{site.data.keyword.baremetal_short}} \n * Dedicated hosts \n * Reservations for virtual servers and bare metal servers \n * Instance Metadata service \n * Instance templates \n * Instance groups \n * Auto Scale for VPC |
| **Performance and availability** | * Networking speeds up to 50 Gbps. For more information, see [Configuring network performance](/docs/virtual-servers?topic=virtual-servers-configuring-network-performance). | * High-speed networking up to 200 Gbps (see [x86-64 instance profiles](/docs/vpc?topic=vpc-profiles)) \n * Zonal architecture provides better availability  |
| **Pricing** | * Hourly and monthly billing \n * Suspend billing feature for supported configurations | * Hourly and monthly billing \n * Suspend billing feature \n * Cost savings for reservations |
| **Bare Metal servers** |  Customizable servers that feature advanced Intel® Xeon® CPUs, or AMD CPUs, and NVIDIA GPUs | Profile-based servers that feature advanced Intel® Xeon® CPUs, Data Processing Unit (DPU) technology, rapid provisioning, and hourly billing  |
| **Virtual server profile families** | * Balanced \n * Balanced local storage \n * Variable compute \n * Compute \n * Memory \n * Transient option for supported profiles \n * GPU | * Balanced \n * Compute \n * Memory \n * Very High Memory \n * Ultra High Memory \n * GPU \n * AI Optimized \n * Storage Optimized \n * Confidential Compute \n * Generations of CPU profiles \n * Profiles for Intel, AMD, and s390x processor architectures  |
| **Supported images** | * Stock images \n * Instance add-ons include OS add-ons, control panel software, and database software \n * Custom images | * Stock images \n * Custom images (includes image from volume) \n * Private catalog images |
| **Platform integration** | | IAM and resource group integration for a unified experience |
{: caption="Compute comparison" caption-side="bottom"}
{: summary="This table has row and column headers. The row headers identify possible features. The column headers identify the differentiators between classic infrastructure and VPC infrastructure. To understand the differences between environments, go to the row and find the details for the feature that you're interested in."}

## Network differentiators
{: #compare-network}

Classic infrastructure relies on physical and virtual network appliances, while VPC infrastructure provides cloud-native network functions that include built-in VPN, load balancing, and network isolation.

| Category   |  Classic infrastructure   | VPC infrastructure |
| ---------- | ------------------------- | ------------------ |
| **Location construct**    | Data centers and Points of Delivery (PODs) \n | Regional model that abstracts infrastructure so you don't need to worry about pod locations.|
| **Network functions and services** |Physical and virtual appliances from multiple vendors | Cloud-native network functions: \n * VPNs \n * Load Balancer as a Service (LBaaS) \n * VPC isolation \n * Multiple vNIC instances \n * Larger subnet sizes |
| **IP addresses** | IPv6 addresses supported | IPv4 addresses only |
| **Gateway routing** | Handled natively by IBM data center routers, or use a network appliance: \n * Virtual Router Appliance \n * Vyatta \n * Juniper vSRX \n * Fortinet FSA | Public gateway and floating IP services handle traffic routing. |
| **Network address translation (NAT)** | Use a virtual or physical network appliance: \n * Vyatta \n * Juniper vSRX \n * Fortinet FSA \n * Fortinet vFSA \n * Bring Your Own Gateway Appliance (BYOGWA) | Supported through floating IP addresses and public gateway functions |
| **IPsec Virtual Private Network (VPN)** | Use a virtual or physical network appliance: \n * Vyatta \n * Juniper vSRX \n * Fortinet FSA \n * Fortinet vFSA \n * BYOGWA | Supported by the VPN-as-a-service offering |
|  **Elastic load balancing** | Cloud Load Balancer  | Load Balancer for VPC |
| **Global load balancing**| Cloud Internet Services, Citrix Netscaler VPX | Cloud Internet Services |
|**Hybrid connectivity** | Direct Link for direct private connectivity from on-premises: \n * Virtual network appliances \n * Physical network appliances (Vyatta, Juniper vSRX, Fortinet FSA, Fortinet vFSA, and BYOGWA) | Connectivity options for on-premises and classic infrastructure resources: \n * Direct Link 2.0 \n * Transit Gateway \n * VPC VPN |
{: caption="Network comparison" caption-side="bottom"}
{: summary="This table has row and column headers. The row headers identify possible features. The column headers identify the differentiators between classic infrastructure and VPC infrastructure. To understand the differences between environments, go to the row and find the details for the feature that you're interested in."}
## Storage differentiators
{: #compare-storage}

Both environments support block and file storage with encryption, snapshots, and adjustable IOPS, but VPC storage adds zonal redundancy, cross-account encryption key authorization, and optional encryption in transit.

|  Classic infrastructure   | VPC infrastructure |
| ------------------------- | ------------------ |
| A robust set of storage services, {{site.data.keyword.blockstorageshort}} (Internet Small Computer Systems Interface (iSCSI)), and {{site.data.keyword.filestorage_short}} (Network File System (NFS)-based) offerings. Server-side agent-based Backup service with dedicated vault. \n - Snapshot support for both offerings. \n - Cross-regional replication. \n - Adjustable input/output operations per second (IOPS) limits and increasable capacity. \n - Supports encryption at rest with provider- or customer-managed keys. \n - Volume duplication and data refresh from parent volume.| {{site.data.keyword.block_storage_is_short}} provides primary boot disks (with basic lifecycle management), and secondary data volumes. {{site.data.keyword.filestorage_vpc_short}} provides NFS-based file shares. \n - Snapshot and backup support for block volumes and file shares. \n - Zonal and cross-regional replication for file shares. \n - Adjustable IOPS and increasable capacity. \n - Supports encryption at rest with provider- or customer-managed keys. \n - Optional encryption in transit for block volumes and file shares. \n - Optional cross-account authorizations for encryption keys and file share access. |
{: caption="Storage comparison" caption-side="bottom"}
{: summary="This table has column headers. The column headers identify the differentiators between classic infrastructure and VPC infrastructure storage. To understand the differences, find the feature in the classic infrastructure column and compare it with the corresponding VPC infrastructure column."}

## Security differentiators
{: #compare-security}

Classic infrastructure uses third-party network appliances for perimeter security, while VPC infrastructure provides built-in security groups and network access control lists for fine-grained traffic control.

|  Classic infrastructure   | VPC infrastructure |
| ---------- | ------------------------- |
|Vyatta, Fortigate, Juniper vSRX, Security Groups for virtual servers| Security groups, Network Access Control Lists (ACLs)|
{: caption="Security comparison" caption-side="bottom"}
{: summary="This table has column headers. The column headers identify the differentiators between classic infrastructure and VPC infrastructure security options. To understand the differences, find the feature in the classic infrastructure column and compare it with the corresponding VPC infrastructure column."}

## API differentiators
{: #compare-apis}

Classic infrastructure uses the SoftLayer API (SLAPI), while VPC infrastructure provides a modern, REST-based API aligned with IBM Cloud platform standards.

|  Classic infrastructure   | VPC infrastructure |
| ------------------------- | ------------------ |
|Existing {{site.data.keyword.slapi_short}} (SLAPI)| New developer-friendly, REST-based API |
{: caption="API comparison" caption-side="bottom"}

## Next steps
{: #compare-nextsteps}

To review all the VPC infrastructure capabilities, see [About virtual private cloud](/docs/vpc?topic=vpc-about-vpc). To start exploring infrastructure overall, see [Building your infrastructure](/docs/overview?topic=overview-get-started-checklist).
