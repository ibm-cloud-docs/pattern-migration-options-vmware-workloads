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

Lift and Shift of the VMware onpremise or collocated platform to Cloud compute aspects focus on the following business requirements:

-   No change to applications in move to cloud
-   Fasttrack a datacenter exit strategy
-   Right size VMware VCF licensed cores
-   Provide inferencing AI compute capabilities
-   Provide a production grade Kubernetes platform

Design Considerations

Target IBM Cloud VCF offering

Rehost and replatform are avoided, with a retain of VMware as the virtualization platform allowing for the same VMware components used in onpremise or collocated facilities. Clients can maintain the same VMware software stack with a lift-and-shift of both the management and workload virtual servers to IBM Cloud VMware Solutions with no application or software changes.

Use of VMware HCX (for VCF) allows for retention of the virtual machine IP addresses and Virtual Machine replication features such as vmotion and storage vmotion allow for live migration of Virtual instances from onPremise or collocated datacenters to IBM Cloud VCF offering.

Choose the right IBM Cloud® for VMware Solutions offering according to

-   the level of VMware management and automation that the customer wants to transfer to IBM Cloud.
-   Level of flexibility to retain same VMWare design, management plane, automation
-   Performance and low latency requirement for workload using 4th generation Intel Xeon

Table here
![Pattern overview.](ibmcloudvcftable.svg "IBM Cloud VMware Solution table"){: caption="Figure 3. IBM Cloud VMware Cloud Foundation Offerings" caption-side="bottom"}

Right size VMware VCF licensed cores

Provide inferencing AI compute capabilities

Provide a production grade Kubernetes platform
