---

copyright:
  years: 2023
lastupdated: "2023-12-26"

subcollection: pattern-migration-options-vmware-workloads

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Migration design
{: #migration-design}



The move of a mission or business critical distributed production platform to IBM Cloud is underpinned by the migration program which we propose to divide into 5 phases: Discovery, Assessment, MVP, Migration and Operate.

Picture here

Discovery Phase1: Data is collected across technical, sales and business teams to understand the motivation and internal factors driving move to Cloud. Identify priorities such as scalability, solving functional issues, lack of in-house skills, reducing infrastructure and IT expenses. Identify and document current infrastructure, applications, relationship, and dependencies including drift from the expected business required state. Key to data collection for the VMware onpremise or collocated platform is to a extraction tool such as RVtools .

Assessment Phase2: Data collected in the discovery phase is used to assess the migration to Cloud viability and choosing the right target platform solution. Prioritise the Lift and Shift migration of the VMWare SDDC to IBM Cloud VMware VCF so that current VMware ISV support, VMWare processes and automation is maintained. Avoid adding re-packaging (applications) or re-factor (to microservices) patterns to decouple the modernize from move to IBM Cloud program. Assess the supply-chain of workload validating utilisation and usage of VMware components. Right-size the target VCF landing zones consolidating VMware clusters making use of higher core density servers. Assess software supply chain and Data for the required encryption level and business key integration. The outcome of the assessment phase is a high-level architecture of the cloud environments with associated bill of materials.

Minimum Viable Product (MVP) Phase3: Provides the confidence in the viability of the proposed solution. It is important to clearly define and articulate upfront the success criteria of the MVP as well as to identify the approving stakeholder(s). The successful MVP will build trust and confidence in the solution and provide the go ahead for the migration of the production workload. The MVP familiarise the operating team with the Cloud platform and guides towards a smooth adoption (transition).

Migration Phase4: Execution of workload (environment) migration. The duration of the migration to IBM Cloud phase is dependent on the complexity and criticality of the production environment. IBM Technology Expert Labs include accelerator services to migrate workload to IBM Cloud.

Operate (run) Phase5: Refers to tasks and processes to maintain the workload operational once the workload has been migrated to the target IBM Cloud VMware platform. Key processes include Backup, Observability (logging / monitoring) and maintaining compliance.
