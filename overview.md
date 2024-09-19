---
copyright:
  years: 2023
lastupdated: "2024-09-19"

subcollection: <repo-name>

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Overview

{: \#overview}

For many enterprises, VMware Software Defined Data Center (SDDC) is the virtualization platform for hosting production business critical distributed (x86-64) workloads in on-premises or in co-located Data Centre facilities.

VMware has 44.8% market share in virtualization platform technologies, per Statista and 79% of Enterprise across globe runs VMware per IDC.

Business challenges are leading clients to re-evaluate the VMware (SDDC) on-premises or collocated platform:

-   Licensing cost increases for VMware virtualization: Businesses are looking to minimize the impact of VMware Cloud Foundation (VCF) bundled pricing changes effective 1 May 2024 and mitigate potential future VCF subscription cost increases. Broadcom introduced a new unified licensing model for VMware software. This new model resulted in businesses needed to fit their current VMware software licences mostly into one of two bundles: VMware Cloud Foundation (VCF) or VMware vSphere Foundation (VVF).
-   High operational costs to maintain on-premises or colocation datacenter facilities: Maintaining compliance, security and growing capacity in on-premise datacenters can lead to significant capital expenditure (CapEx) and operating expenditure (OpEx) making release of funding for business innovation challenging.

    Maintaining compliance and security costs include

    -   Managing costly compliance (update certifications) and audits
    -   Shorter server refresh cycles to avoid costly extended warranty
    -   Time consuming Server and VMware SDDC security patching updates

        Growing on-premises capacity challenges include

    -   Slow (multi-week) new VMware ESX server provisioning for new capacity requirements
    -   Slow increased server memory (RAM) or additional storage request execution

        In addition, businesses faced with growing cybersecurity threads and data breaches are requiring their CISO to adopt the National Institute of Standards and Technology (NIST) cybersecurity best practices and apply adequate preventative and recovery security measures to their systems.

-   Deliver improved platform availability, resiliency, performance and scaling business requirements due to the accelerated shift to a digital economy. There has been a substantial increase in users working remotely from home, which started during the COVID-19 pandemic and has continued since. This has led to an increased use of web-based and mobile applications. Due to this, business systems that once needed to be available 8 hours per day 5 days per week (8x5) now need to be available 24x7 with platform availability of 99.99%+. Cloud providers such as IBM can provide higher availability at lower costs than businesses can typically do on premise.
-   Slow innovation and deployment of new modernized (cloud native) applications or services: initial application modernization to the cloud native operating system (Linux) and container platform (Kubernetes) was very successful for Web applications but have struggled particularly with modernization of Windows .Net Framework applications, leading to delayed application modernization (to cloud native) development programs
-   Delayed implementation of a datacentre exit business mandate.
-   Deploying zero trust security model across hybrid cloud.

This whitepaper proposes to retain the VMware platform, leverage seamless migration standard tools (such as VMware HCX) to lift and shift the hosted business workloads (no application changes) into IBM Cloud VMware Solutions.

![Pattern overview.](Overview.svg){: caption="Figure 1. Lift and Shift VMware business workloads to IBM Cloud VMware Solutions." caption-side="bottom"}

Moving mission and business critical VMware workload environments to IBM Cloud VMware Solutions enables the following benefits:

-   Enterprise-grade Cloud Infrastructure – leverage IBM Cloud robust and secure infrastructure designed to meet the stringent requirements of mission and business critical workloads.
-   Flexibility – access to wide variety of hardware (chipsets) profiles including latest Intel Xeon processors (currently 4th Gen.), access to VMware compute accelerators including network uplinks 100 Gb/s, enabling higher virtual instance densification, CPU utilization. Scaling capacity on VPC offerings allow for new capacity with the hour.
-   Opportunity to move VMware managed services and VMWare automation asset maintenance to IBM Cloud VMWare Cloud Foundation as a Service (including DRaaS).
-   Advanced Cloud Services – access to latest GPUs such as Nvidia for AI client solutions along with IBM Watsonx services (GenAI (encoder / decoder / LLMs) and Machine Learning) to drive innovation into business processes.
-   Optimize Distributed Workload – in move to IBM Cloud there is further opportunity to optimize the x86-64 workload to alternative IBM cloud enabled virtualization platforms such as KVM, Xen, PowerVM.
-   Cost savings – avoid unnecessary expenses associated with re-purchasing licenses for new infrastructure when adopting the new Broadcom / VMware VCF subscription. VMware Cloud Foundation on IBM Cloud allows businesses to address Broadcom Licensing immediately and generate a a better near-term ROI, which can then be redirected towards future re-hosting, re-platforming or application modernization to microservices initiatives.

![Pattern overview.](ibmcloudvcfroi.svg){: caption="Figure 1. A description that prints on the page" caption-side="bottom"}

Figure 2 Generating return on investment with move to IBM Cloud VMware solutions.

The whitepaper describes the design solution considerations, migration program approach and key architecture decisions to fasttrack a move of the On Premise or Co- Located VMware platform and hosted environments (PROD, NONPROD, TEST, DEV) to IBM Cloud VMware Solutions using lift-and-shift with no change to the business applications.
