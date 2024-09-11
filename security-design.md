---

copyright:
  years: 2024
lastupdated: "2024-09-11"

subcollection: pattern-sap-on-vpc

keywords:

---

{{site.data.keyword.attribute-definition-list}}

# Security Considerations
{: #security-design}


The following table summarizes the security design considerations when solutioning IBM Cloud VMware Solutions for lift and shift VMware on-premises Workload into IBM Cloud with consideration for adopting the National Institute of Standards and Technology (NIST) cybersecurity best practices.

**Requirements**

-   Adopt and implement a Zero trust security strategy
-   Integrate IBM Cloud IAM with the enterprise LDAP directory service
-   Provide relevant industry compliant compute platform
-   Provide a Key Management System for data encryption
-   For mission and business critical workloads provide client encryption key retension solution.

| Security Areas                     | Description                                                                                                                                                                                                                                                                                                                                     |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Adopt Zero trust security strategy | Base implementation on Principle of duty segregation, Role based access control (RBAC), verification on access. Segregation of duty ensures network, compute and storage administrators use separately defined RBACs. Additionally, Developers do not have access to production. All access to and changes to resources are secure and audited. |
| Data encryption                    | In transit encryption is enabled to prevent interception and tampering. Data at-rest encryption is enabled for backup and  virtual disks. Application data use secure communication protocols like TLS.                                                                                                                                               |
|                                    |                                                                                                                                                                                                                                                                                                                                                 |
