---
copyright:
  years: 2023
lastupdated: "2023-12-26"

subcollection: pattern-migration-options-vmware-workloads

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Architecture decisions for compute

{: \#compute-decisions}

| Architecture decision | Requirement                                                                                | Options                                                                                                                                                             | Decision                       | Rationale                                                                                                  |
|-----------------------|--------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------|------------------------------------------------------------------------------------------------------------|
| Virtualization        | - No change to applications in move to cloud\n. - Fasttrack datacentre exit strategy\n.    | IBM Cloud VMware offerings. Re-platform to public cloud KVM virtual instance. Nutanix on-premises. Re-platform to public cloud KubeVirt Virtual Instance Container. | IBM Cloud VMware Offerings.    | Retain VMware hypervisor, use VMware HCX for seamless (no application change) lift and shift move to Cloud |
| Availability          | Mission Critical, Business Critical VMware platform availability 99.99% with near zero RPO | Deploy IBM Cloud VMware Cloud Foundation in IBM Cloud Single Availability region 2 Deploy IBM Cloud VMware Cloud Foundation in IBM Cloud Multi Zone Region          | IBM Cloud Multi Zone Region    |                                                                                                            |
| VMware lifecycle      | For Test and Dev environments Leverage Cloud Provider VMWare Automation and Services       | 1 IBM Cloud VMware VCF aaS Single Tenant 2 IBM Cloud VMware VCF aaS Multi-tenant                                                                                    | IBM Cloud VCF aaS multi-Tenant |                                                                                                            |
| Containers            | text                                                                                       | text                                                                                                                                                                | text                           | text                                                                                                       |

{: caption="Table 1. Architecture decisions for compute" caption-side="bottom"}
