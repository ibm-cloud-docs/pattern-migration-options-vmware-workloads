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

-   Fasttrack a datacenter exit strategy
-   Provide secure internet access to Web applications
-   For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.
-   Provide secure administrative access to VMware Cloud Foundation
-   Provide global load balancer capability for Web applications
-   For regulated, mission and business critical workloads provide DMZ

    **Optional requirements**

-   Provide integration with on-premise Microsoft Active Directory
-   

## Design Considerations

| Network Areas                                                | Description               |
|--------------------------------------------------------------|---------------------------|
| Choosing the IBM Cloud region                                |                           |
|                                                              |                           |
| Lift and Shift of DMZ                                        |                           |
| Firewall / Router                                            |                           |
|                                                              |                           |
| Interconnectivity between IBM VMware Solutions and IBM Cloud | Multiple VMware Solutions |
| DNS                                                          |                           |
| Global Load Balancer                                         |                           |
