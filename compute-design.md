---

copyright:
  years: 2023
lastupdated: "2023-12-28"

subcollection: pattern-migration-options-vmware-workloads

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Compute design 
{: #compute-design}


The following are compute design requirements and considerations for lift and shift VMware workloads to IBM Cloud.

Requirement

Requirements for compute aspects for lift and shift to secure cloud focusses on the following:

-   No change to applications in move to cloud
-   Fasttrack the datacenter exit strategy
-   Right size VMware VCF licensed cores
-   Provide inferencing AI compute capabilities
-   Provide a production grade Kubernetes managed platform
-   Provide Cloud native x86-64 compute with integration into GitOps and CI/CD pipelines

Design Considerations

Rehost and replatform are avoided, with a retain of VMware as the virtualization platform allowing for the same VMware components used in onpremise or collocated facilities. Clients can maintain the same VMware software stack with a lift-and-shift of both the management and workload virtual servers to IBM Cloud VMware Solutions with no application or software changes.

Use of VMware HCX (for VCF) allows for retention of the virtual machine IP addresses and Virtual Machine replication features such as vmotion and storage vmotion allow for live migration of Virtual instances from onPremise or collocated datacenters to IBM Cloud VCF offering.

Choosing the right IBM Cloud® for VMware Solutions offering according to the level of VMware management and automation that the customer wants to transfer to IBM Cloud.

Table here

Requirement Right size VMware VCF licensed cores

Text from Chuck here

Requirement

Provide inferencing AI compute capabilities

VSIs with GPUs
