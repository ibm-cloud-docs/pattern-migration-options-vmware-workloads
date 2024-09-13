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

| Storage Areas                                                                       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Fasttrack datacentre exit and move to cloud                                         | The migration of the VMware datastores from on-premise to IBM Cloud is covered by the migration program. Two methods can be assessed: cold migration of virtual instances or live migration of virtual instances using VMware storage vmotion. Most migration programs will use cold migration as VMware Storage vmotion has many requirements.                                                                                                                                                              |
| Mission and business critical VMware Storage for 99.99% Availability and RPO near 0 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Replacing on-premises tape or long term storage                                     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Optimize VMware storage Operational and Capital costs                               | When moving to IBM Cloud VMware solutions Operational expenses cost reductions are achieved through replacing or reducing significantly manual tasks such as storage deployment, compliance configuration, scaling and capacity expansion with storage policies defined within VCF.  When using vSAN storage policies for compliance and deployment   When using NFS File Storage from IBM Cloud  All storage admin by IBM Cloud When using Block storage by IBM Cloud all admin by IBM Cloud  CapEx … zero  |
