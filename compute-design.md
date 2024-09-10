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


The following table summarizes the compute design considerations when solutioning lift and shift VMware on-premise workloads to IBM Cloud VMware Solutions.

**Requirements**

-   No change to applications in move to cloud
-   Fasttrack a datacenter exit strategy
-   Right size VMware VCF licensed cores
-   For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.

**Business innovation requirements**

-   Enable AI inferencing in production business processes
-   Provide encoder / decoder capabilities for GenAI business process innovation development
-   Provide mission and business critical Kubernetes platform for modernized cloud native applications


**Design Considerations**

| Compute Areas                                     | Description                                                                                                                                                                                                                                                                                                                                                                        |
|---------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Retain VMware Virtualization                      | Rehost and replatform are avoided, with a retain of VMware as the virtualization platform allowing for the same VMware components used in onpremise or collocated facilities. Clients can maintain the same VMware software stack with a lift-and-shift of both the management and workload virtual servers to IBM Cloud VMware Solutions with no application or software changes. |
| Choosing IBM Cloud® for VMware Solutions offering | The level of VMware management and automation that the customer wants to transfer to IBM Cloud.  Level of flexibility to retain same VMWare design, management plane, automation.  Performance and low latency requirement for workload using 4th generation Intel Xeon.                                                                                                           |
| Right Sizing VMware VCF License core              |                                                                                                                                                                                                                                                                                                                                                                                    |
| Migration tooling                                 | VMware HCX (for VCF) allows for retention of the virtual machine IP addresses and Virtual Machine replication features such as vmotion and storage vmotion allow for live migration of Virtual instances from onPremise or collocated datacenters to IBM Cloud VCF offering.                                                                                                       |

Table here
![Pattern overview.](ibmcloudvcftable.svg "IBM Cloud VMware Solution table"){: caption="Figure 3. IBM Cloud VMware Cloud Foundation Offerings" caption-side="bottom"}

Right size VMware VCF licensed cores

Provide inferencing AI compute capabilities

Provide a production grade Kubernetes platform
