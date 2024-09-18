---
copyright:
  years: 2024
lastupdated: "2024-09-11"

subcollection: pattern-sap-on-vpc

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Security Considerations

{: \#security-design}

The following table summarizes the security design considerations when solutioning IBM Cloud VMware Solutions for lift and shift VMware on-premises Workload into IBM Cloud with consideration for adopting the National Institute of Standards and Technology (NIST) cybersecurity best practices.

## Security Requirements

-   Adopt Zero trust security strategy
-   Integrate IBM Cloud IAM with the enterprise LDAP directory service
-   Provide relevant industry compliant IBM Cloud VMware solution platform
-   Provide a Key Management System for data encryption
-   For mission and business critical workloads provide client encryption key retention solution.

## Security Considerations

| Security Areas               | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Adopting Zero trust | Follow the principle of duty segregation using Role based access control (RBAC). Segregation of duty ensures network, compute and storage administrators use separately defined RBACs. Additionally, Developers do not have access to production. <br> Implement principle of least privilege by assigning only required access permissions. A time-based conditional access can be granted to limit access to timeframe you specify reducing opportunity for attack in the event of security breach. <br> Access to and changes to resources including applications, compute, network, storage  are secured, audited and verified.  |
| Single Sign On               | Many enterprises use Microsoft Active Directory as the LDAP for the corporate (or business) identity provider (IdP). Review the ability to federate your corporate identity provider (IdP) with IBM Cloud IAM to allow your employees access to IBM Cloud with the company username and password (SSO).                                                                                                                                                                                                                                                         |
| Privileged access management | Administrative access to the IBM Cloud VMware Solutions is restricted, audited and logged via a bastion host solution.                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Data encryption              | In transit encryption is enabled to prevent interception and tampering. Data at-rest encryption is enabled for backup and virtual disks. Application data use secure communication protocols like TLS.                                                                                                                                                                                                                                                                                                                                                          |
| Compliance                   | Regulatory compliance: ensure the IBM Cloud VMware solution adheres to relevant industry regulations and compliance standards, such as GDPR, HIPAA, or any other applicable requirements.                                                                                                                                                                                                                                                                                                                                                                       |
