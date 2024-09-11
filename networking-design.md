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

**Requirements**

-   Fasttrack a datacenter exit strategy
-   For Mission and Business critical workloads deliver 99.99% Availability and RPO near zero.
<p>



**Design Considerations**


| Network Areas                                                 | Description                              |
|---------------------------------------------------------------|------------------------------------------|
| Choosing the Cloud location                                   |                                          |
| Choosing between Classic and VPC                              | VPC for lowest latency highest bandwidth |
| Lift and Shift of DMZ                                         |                                          |
| Firewall / Router                                             |                                          |
|                                                               |                                          |
| Interconnectivity between IBM VMware Solutions and IBM Cloud  | Multiple VMware Solutions                |
| DNS                                                           |                                          |
| Load Balancer                                                 |                                          |
