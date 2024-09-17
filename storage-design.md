---
copyright:
  years: 2023
lastupdated: "2023-12-26"

subcollection: pattern-sap-on-vpc

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Storage Considerations

{: \#storage-design}

## Storage Requirements

The storage requirements for the lift and shift VMware to IBM Cloud VMware solution focus on the following

Fasttrack a datacentre exit strategy with move VMware workloads to cloud.

Replace on-premises VMware storage solution.

Optimize VMware storage operational expense (OpEx) and Capital expenditure (CapEx)costs.

For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.

Provide replacement for on-premises tape backup storage.

Provide secure automated backup service.

## Storage Design Considerations

| Storage Areas                                                                       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| IBM Cloud Storage Options                                                           | The options for storage for VMware solutions on IBM Cloud are IBM Cloud File or Block, vSAN and Cloud Object Storage. With the new VCF licensing bundle, vSAN software is included by default and 1 TiB per core of vSAN storage is included. This makes vSAN more economical than Block or File in most cases. IBM Cloud Object Storage is best suited for unstructured data and long term or archival data storage. IBM Block and File storage offer scalable storage without having to scale compute nodes. However, they do not have the same resiliency options, such as (geographically) stretched clusters as vSAN. vSAN scales differently from Block and File. It is a hyperconverged architecture for which compute and storage reside in the same node thereby which requires additional compute nodes to increase storage capacity.  |
| Fasttrack datacentre exit and move to cloud                                         | The migration of the VMware datastores from on-premises to IBM Cloud is covered by the migration program.  For migrations to IBM Cloud VCF, VMware HCX, PrimaryIO or third party services can be used.  For migrations to VMware as a Service, VMware Cloud Director for Availability (VCDA) is used.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| Mission and business critical VMware Storage for 99.99% Availability and RPO near 0 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Replacing on-premises tape or long term storage                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Optimize VMware storage Operational and Capital costs                               | When moving to IBM Cloud VMware solutions Operational expenses cost reductions are achieved through replacing or reducing significantly manual tasks such as storage deployment, compliance configuration, scaling and capacity expansion with storage policies defined within VCF. When using vSAN storage policies for compliance and deployment When using NFS File Storage from IBM Cloud All storage admin by IBM Cloud When using Block storage by IBM Cloud all admin by IBM Cloud CapEx … zero                                                                                                                                                                                                                                                                                                                                           |
