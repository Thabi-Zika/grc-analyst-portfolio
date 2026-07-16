# PROJECT 3: INFORMATION SECURITY ACCESS CONTROL POLICY

1. Document Control Metadata
* Document ID: POL-SEC-04
* Version: 1.0  
* Classification: Internal Use Only  
* Effective Date: 16 July 2026  
* Review Cycle: Annual  
* Framework Alignment: ISO/IEC 27001:2022 (Controls A.5.15 - A.5.18), NIST CSF v2.0 (PR.AA)



2. Role-Based Access Control (RBAC) Authorization Matrix

| Predefined Job Role | Permitted Access Scope | Prohibited Access Scope |
| :--- | :--- | :--- |
| **Logistics Coordinator** | Read and write access to shipping manifests, route-optimisation logs, and warehouse inventory databases. | Strictly prohibited from accessing customer financial wallets, change-billing scripts, or database source code. |
| **FinTech Systems Engineer** | Full administrative access to deploy CI/CD pipeline code, manage cloud server infrastructure, and monitor system performance logs. | Strictly prohibited from viewing raw, plaintext cardholder data (PAN) or exporting customer PII databases. |



3. Core Policy Directives

3.1 Principle of Least Privilege
* Access permissions must be strictly restricted to the minimal rights necessary for an individual to execute their explicit professional responsibilities.
* The default state for all corporate access control systems shall be set to 'Deny All'.

3.2 User Access Reviews (UAR)
* **Standard Accounts:** Line managers and compliance teams must audit standard employee access rights every 90 days.
* **Privileged Accounts:** Highly privileged accounts (e.g. Domain Administrators, Root database users) must be audited every 30 days.
* Any discovered access discrepancies or 'privilege creep' must be revoked within 24 hours of identification.

3.3 Offboarding and Access Revocation
* Upon an employee's formal resignation, termination, or contract conclusion, Human Resources must immediately alert the IT Security team.
* All logical access privileges (corporate email, VPN access, SSH keys, and SaaS tools) must be systematically disabled within a maximum of 2 hours of the employee's formal departure time to mitigate insider threat risks.



**Policy Approver:** [Nthabeleng Thebehadi], GRC Analyst Trainee
