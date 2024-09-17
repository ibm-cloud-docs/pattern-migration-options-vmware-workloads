---
copyright:
  years: 2023
lastupdated: "2023-12-26"

subcollection: pattern-sap-on-vpc

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Network Considerations

{: \#network-design}

The following table summarizes the network design considerations when solutioning lift and shift VMware on-premise workloads to IBM Cloud VMware Solutions.

## Network Requirements

- Provide secure access to Web applications from internet
- For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.
- Provide secure connectivity between customer remaining Onpremise and VMware Cloud Foundation on IBM Cloud
- Provide global load balancer capability for Web applications
- For regulated, mission and business critical workloads provide DMZ

    **Optional requirements**

- Provide integration with on-premise Microsoft Active Directory

## Design Considerations

| Network Areas                                                                                              | Description                                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Choosing the IBM Cloud region                                                                              | Decide if the VCF instance will be deployed in a multi zone region (MZR) or in a single zone region (SZR). Using an MZR enables to achieve a higher level of availability/resiliency through the deployment of at least two VCF instances in two different availability zones. Note that if vSAN is used, cross availability zone replication is possible but requires a witness running in a third availability zone (the witness can consist in a small IBM Cloud virtual server instance).                                                                                             |
| Provide secure connectivity between customer remaining On-premise and VMware Cloud Foundation on IBM Cloud | To securely connect from the remaining on-premises environment to the IBM Cloud environment IBM Cloud Direct link or VPN connectivity can be used. IBM Cloud Direct link is a high capacity private connection while VPN connectivity consists in an encrypted site-to-site or client-to-site tunnel over the public internet. On the IBM Cloud side, the termination point for both options will depend on the level of isolation required inside the IBM Cloud environment and on the VCF deployment flavor. For more information regarding IBM Cloud Direct Link and VPN options see [IBM Cloud Direct Link](https://cloud.ibm.com/docs/dl?topic=dl-get-started-with-ibm-cloud-dl), [IBM Cloud VPNaaS](https://cloud.ibm.com/docs/vpc?topic=vpc-vpn-overview) and [IBM CLoud CLassic VPN options](https://cloud.ibm.com/docs/iaas-vpn?topic=iaas-vpn-getting-started)                                                                                                                                        |
| Provide secure and available access to Web applications from internet                                      | To secure or filter traffic entering the environment, capabilities such as DDoS mitigation or web application firewall (WAF) should be considered. IBM Cloud Internet Services (CIS) includes these capabilities as well as has the capability to act as a global load balancer (GLB), allowing to increase the availability/resiliency of the workloads running on VCF on IBM Cloud, provided that at least two different instances are deployed in at least two different availability zones. Alternatively, third party GLBs can also be used. For more information on IBM Cloud Internet Services see [IBM CIS](https://cloud.ibm.com/docs/cis?topic=cis-getting-started)                                                                 |
| Firewall                                                                                                   | When migrating from on premises to VCF on IBM Cloud, the firewall constructs available within the VMware environment remain unchanged, however particular attention should be given to the firewalling at the edge of the VMware environment. The recommended approach is to use a similar type of firewall appliance in IBM Cloud as the one used on-premises to limit the operational changes, leverage the skills of existing operations team and and therefore minimize the risk of disruption. <br> Another point to consider is the firewall availability/resiliency requirements, especially in the case of IBM Cloud VPC as the HA modes that are supported will vary based on the firewall appliance type.<br>Several firewall virtual or physical options are available for IBM Cloud VPC (Juniper vSRX, Fortinet vFSA, F5 Big-IP VE, Palo Alto VM-Series) and IBM Cloud Classic (Juniper vSRX, Fortinet FSA and vFSA, Vyatta Virtual Router Appliance). It is also possible to bring your own gateway (as a virtual appliance on top of a dedicated IBM Cloud Classic bare metal or as an IBM Cloud VPC VSI deployed from a custom image). |
| Interconnectivity within IBM Cloud                                                                           | IBM To reach the various IBM Cloud Services from the VCF on IBM Cloud environment, Virtual Private Endpoints (VPE) or Cloud Service Endpoints (CSE) can be used, depending on if the VCF on IBM Cloud instance is located in IBM Cloud Classic or in IBM Cloud VPC. Both VPEs and CSEs allow to privately reach the IBM Cloud services, keeping the traffic within IBM Cloud and avoiding any egress traffic charges. For more information on VPEs and CSEs, see [IBM Cloud VPE](/docs/vpc?topic=vpc-about-vpe) and [IBM Cloud CSE](https://cloud.ibm.com/docs/account?topic=account-service-endpoints-overview) <br> Integration of the different IBM Cloud IaaS (VPC, classic and PowerVS) is achieved by using the IBM Cloud Transit Gateway, which is a as a service BGP router that can also be used as the termination point for direct link connectivity. IBM Cloud transit gateway can be local, limited to a specific region or global, spanning multiple regions. For more information on IBM Cloud Transit Gateway see: [IBM Cloud Transit Gateway](/docs/transit-gateway?topic=transit-gateway-getting-started)                                                                |
