---
copyright:
  years: 2023
lastupdated: "2023-12-18"

subcollection: pattern-vpc-vsi-multizone-resiliency

keywords:
---

# IBM Cloud Hypervisor

**Description**

Virtual instances are converted to Linux Hypervisor format, with Linux hypervisor managed by IBM Cloud.

The IBM Cloud Hypervisor should be considered for workloads where client wants to remove the VMware dependencies.

**Requirements**

Reduce exposure to potential further increases in VMware Cloud Foundation license cost

Implement strategy to move away from VMware hypervisor

Deploy and lifecycle virtual instances using cloud automation

**Design Considerations**

| Re-platform Virtual Machine to alternate hypervisor  | Consider re-configuration of virtual server in choosing the right workload to re-platform.  Requirement for re-design of Network configuration (including potential IP address change) can lead to complexity and delays in conversion.                                                                                                           |
|------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Virtual instance lifecycle automation                | Deployment, scaling, patching automation built up with VMware API will need to be developed with Terraform and Ansible.                                                                                                                                                                                                                           |
| Replacing VMware management stack                    | Additional IBM Cloud services will be required to provide comparable VMware capabilities.                                                                                                                                                                                                                                                         |
| Migration Tooling                                    | To implement a migration from On-premise VMware to IBM Cloud Virtual Server Instance, the RackWare Management Module (RMM) migration solution provides a seamless virtual-to-virtual replatforming for VMware virtual machine (VM) to IBM Cloud® virtual server instance migration. It allows the adoption of existing capabilities of IBM Cloud. |

References

[About virtual server instances for VPC \| IBM Cloud Docs](https://cloud.ibm.com/docs/vpc?topic=vpc-about-advanced-virtual-servers&interface=ui)

Deployable pattern

[VSI on VPC landing zone](https://cloud.ibm.com/docs/deployable-reference-architectures?topic=deployable-reference-architectures-vsi-ra-qs)

|   |   |   |   |   |
|---|---|---|---|---|
