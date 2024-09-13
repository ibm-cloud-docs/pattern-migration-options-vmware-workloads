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

-   Provide secure access to Web applications from internet
-   For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.
-   Provide secure connectivity between customer remaining Onpremise and VMware Cloud Foundation on IBM Cloud
-   Provide global load balancer capability for Web applications
-   For regulated, mission and business critical workloads provide DMZ

    **Optional requirements**

-   Provide integration with on-premise Microsoft Active Directory
-   

## Design Considerations

| Network Areas                                                                                              | Description                                                                                                                                                                                                                                                                                         |
|------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Choosing the IBM Cloud region                                                                              | MZR or Single region. Explain how to operate to SLA level … requires several instances of VCF in separate Cloud DCs.  For vSAN Witness can be deployed as IBM Cloud VSI.  Link                                                                                                                      |
| Provide secure connectivity between customer remaining On-premise and VMware Cloud Foundation on IBM Cloud | Direct link or VPN…. Termination point for both will depend on level of isolation required, VCF deployment flavor.                                                                                                                                                                                  |
| Provide secure and available access to Web applications from internet                                      | Support for DDOS mitigation.  Incoming traffic filtering. WAF.  Consider is CIS or 3rd existing.  CIS has GLB capability would need workloads in either multi az or regions for increased HA.                                                                                                       |
| Firewall                                                                                                   | High level view of considerations when doing the shift  You look to replace the equivalent hardware or Virtual instance applicance from On Prem IF it exists in the IBM Cloud catalog OR BYOGateway for Classic or VNF in VPC  Main impact is HA of the FW itself … for VPC  Keep it short Bertand  |
| Interconnectivity with IBM Cloud                                                                           | IBM Cloud Services – VPE (VPC) CSE (Classic) Links to be included  For IBM Cloud IaaS interconnectivity  Use of transit gateway for PowerVS or Classic / vpc integration.  Links to be included Bertrand                                                                                            |
