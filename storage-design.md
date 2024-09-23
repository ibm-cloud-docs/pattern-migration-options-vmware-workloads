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

{: \#storage-requirements}

* Fast track datacenter exit by moving VMware workloads to cloud.

* Replace the on-premises VMware storage solution.

* Optimize VMware storage operational expense (OpEx) and Capital expenditure (CapEx) costs.

* For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.

* Provide replacement for on-premises tape backup storage.

* Provide secure automated backup service.

Storage Design Considerations

| Storage Areas                                         | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|-------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| IBM Cloud Storage Options                             | The options for storage for VMware solutions on IBM Cloud are IBM Cloud File or Block, vSAN and Cloud Object Storage. With the new VCF licensing bundle, vSAN software is included by default and 1 TiB per compute core of vSAN storage is included. This makes vSAN more economical than Block or File in most cases. IBM Cloud Object Storage is best suited for unstructured data and long term or archival data storage. IBM Block and File storage offer scalable storage without having to scale compute nodes. However, they do not have the same resiliency options, such as (geographically) stretched clusters as vSAN. vSAN scales differently from Block and File. It is a hyperconverged architecture for which compute and storage reside in the same node which requires additional compute nodes to increase storage capacity. |
| Backup and Disaster Recovery                          | Disaster Recovery tools - IBM Cloud offers a variety of IBM and third party tools for backup and disaster recovery of VMWare workloads

Veeam - enables Availability with integrated backup, recovery and replication on IBM Cloud. Veeam delivers efficient agentless backups and disaster recovery of IBM Cloud for VMware Solutions workloads and flexible recovery from IBM Cloud backup repositories. Veeam on IBM Cloud seamlessly integrates directly with VMware hypervisors to help achieve high availability. This service provides recovery points and time objectives for your applications and data. The recovery points and time objectives can be provided in less than 15 minutes after configuration is completed. 
/docs/vmwaresolutions?topic=vmwaresolutions-veeamvm_overview

VMWare Cloud Director Availability (VCDA) -VCDA can be installed on a VMware Cloud Foundation as a Service (VCFaaS) instance to create a disaster recovery configuration. Using the VCDA service, you can replicate the primary production workload environment over to a failover environment during an unplanned service interruption. When the interruption resolves, the workload moves back to the primary environment. 
/docs/vmwaresolutions?topic=vmwaresolutions-vmware-aas-overview&q=VCDA&tags=vmwaresolutions


Zerto - provides on-premise and IBM Cloud customers with a secure, flexible and scalable Disaster Recovery solution. It is a single tenant solution for VCF on both Classic and VPC environments in IBM Cloud the provisioning process is fully automated, and the environment is rapidly deployed to the IBM Cloud. Zerto is a Pay-As-You-Go flexible solution that allows you to scale compute capacity horizontally. 
/docs/vmwaresolutions?topic=vmwaresolutions-addingzertodr

ProtectIO – a Disaster Recovery as a Service (DRaaS) offering from PrimaryIO that runs natively on IBM Cloud. ProtectIO enables near zero Recovery Point Object (RPO), which ensures minimal to no loss. It performs continuous replication which does not need scheduling, agents, or appliances. Its agentless protection technique has no impact on the performance of the primary site.
https://www.primaryio.com/protectio/

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| Optimize VMware storage Operational and Capital costs | When moving to IBM Cloud VMware solutions Operational expenses cost reductions are achieved through replacing or reducing significantly manual tasks such as storage deployment, compliance configuration, scaling and capacity expansion with storage policies defined within VCF. When using vSAN storage policies for compliance and deployment When using NFS File Storage from IBM Cloud All storage admin by IBM Cloud When using Block storage by IBM Cloud all admin by IBM Cloud CapEx … zero                                                                                                                                                                                                                                                                                                                                          |
