---

copyright:
  years: 2023
lastupdated: "2023-11-28"

subcollection: <repo-name>

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Overview
{: #overview}



For many enterprises, VMware Software Defined Data Center (SDDC) is the virtualization platform for hosting mission or business critical production distributed (x86-64) workloads in on-premises or co-located Data Centre facilities.

VMware has 44.8% market share in virtualization platform technologies, per Statista and 79% of Enterprise across globe runs VMware per IDC.

Business challenges are leading clients to re-evaluate the VMware (SDDC) on-premises or collocated platform:

-   Licensing cost increases for VMware virtualization: Businesses are looking to minimize the impact of VMware Cloud Foundation (VCF) bundled pricing changes effective 1 May 2024 and mitigate potential future VCF subscription cost increases. The new model resulted in businesses needed to fit their current VMware software licences mostly into one of two bundles: VMware Cloud Foundation (VCF) or VMware vSphere Foundation (VVF).
-   High operational costs to maintain on-premises or colocation datacenter facilities: Maintaining compliance, security and growing capacity in on-premise datacenters can lead to significant capital expenditure (CapEx) and operating expenditure (OpEx) making release of funding for business innovation challenging. Maintaining compliance and security costs include
    -   Managing costly compliance (update certifications) and audits
    -   Shorter server refresh cycles to avoid costly extended warranty
    -   Time consuming Server and VMware SDDC security patching updates

        Growing on-premises capacity challenges

    -   Slow (multi-week) new VMware ESX server provisioning for new capacity requirements
    -   Slow increased server memory (RAM) or additional storage request execution

        In addition, businesses are faced with growing cybersecurity threads and data breaches requiring investment in security skills, processes and automation.

-   Deliver the platform availability, resiliency, performance and scaling business requirements: The accelerated shift to a digital economy, partly due to the Covid pandemic, along increased business demand for higher availability of production critical applications requires greater platform availability of 99.99+%.
-   Slow innovation and deployment of new modernized (cloud native) applications or services: initial application modernization to the cloud native operating system (Linux) and container platform (Kubernetes) was very successful for Web applications but have struggled particularly across .Net Framework applications, leading to delayed application modernization (to cloud native) development programs
-   Costly implementation of Cloud First, Move to Cloud strategies or datacentre exit mandates.

This whitepaper proposes to retain the VMware platform, leverage seamless migration standard tools (such as VMware HCX) to lift and shift the hosted business workloads (no application changes) into IBM Cloud VMware Solutions enabling businesses to access the following benefits:

-   Flexibility – access to wide variety of hardware (chipsets) profiles including latest Intel Xeon processors (currently 4th Gen.) enabling optimized compute utilization and scale the IT requirements.
-   Cost savings – avoid unnecessary expenses associated with re-purchasing licenses for new infrastructure when adopting the new Broadcom / VMware VCF subscription.
-   Opportunity to move VMware services (exit VMware skill risk) to IBM Cloud through VCFaaS (including DRaaS).
-   Enterprise-grade Cloud Infrastructure – leverage IBM Cloud robust and secure infrastructure designed to meet the stringent requirements of mission and business critical workloads.
-   Advanced Cloud Services – access to latest GPUs such as Nvidia for AI client solutions along with IBM Watsonx services (GenAI (encoder / decoder / LLMs) and Machine Learning) to drive innovation into business processes.
-   Optimize Distributed Workload – in move to IBM Cloud there is further opportunity to optimize the x86-64 workload to alternative IBM cloud enabled virtualization platforms such as KVM, Xen, PowerVM.

Here is the Overview diagram that provide details on the ................

![Pattern overview.](Overview.svg "Title text that shows on hover here"){: caption="Figure 1. A description that prints on the page" caption-side="bottom"}

This whitepaper describes the design solution considerations with moving the VMware On Premise or Co- Located environments (PROD, NONPROD, TEST, DEV) to IBM Cloud VMware Solutions using lift-and-shift (no change) of the business applications.

The lift and shift (no change to applications) strategy of workload move to IBM Cloud is chosen to allow for a short (starting less than 6 months) migration program to a target IBM Cloud VMware landing zone. Short migration programs allow for timely return on investment and releasing funding for application modernization and business innovation.
