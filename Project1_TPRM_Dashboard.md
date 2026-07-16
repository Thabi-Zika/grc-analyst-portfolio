# PROJECT 1: SUPPLY CHAIN & THIRD-PARTY RISK MANAGEMENT (TPRM) DASHBOARD

1. Project Context
* **Target Industries:** Logistics & FinTech (Supply Chain Security / B2B SaaS Vendor Risk)
* **Framework Mapping:** NIST CSF v2.0 (GV.SC), ISO/IEC 27001:2022 (A.5.19), COBIT 2019 (APO10)
* **Scenario:** A global logistics platform is onboarding RouteSmart SaaS, a cloud-based third-party vendor handling real-time delivery route optimisation, API integrations, and fleet coordinates. This assessment evaluates their security posture prior to processing live production data.




2. Vendor Inventory Database Schema

| Vendor Name | Service Provided | Data Types Handled | Criticality Rating | Assessment Status |
| :--- | :--- | :--- | :--- | :--- |
| **RouteSmart SaaS** | AI Route Optimisation | Customer Names, GPS Coordinates, Fleet API Keys | **High** | Under Evaluation |
| **PayGate API** | Merchant Credit Card Processing | Cardholder Data (PAN), Billing Addresses, PCI Data | **Critical** | Approved |
| **LogiTrack IoT** | Telematics Tracking | Hardware Serial Numbers, Fleet Location Logs | **Medium** | Approved |



3. Security Questionnaire & Control Mapping

| Control Domain | Security Question | Vendor Response | Mapped Control | GRC Analyst Remediation Action |
| :--- | :--- | :--- | :--- | :--- |
| **Access Control** | Is Multi-Factor Authentication (MFA) enforced for all employees accessing customer data? | No | PCI-DSS v4.0 Req 8.3 / ISO A.8.5 | **CRITICAL GAP:** Mandate MFA implementation within 30 days before full API connection is approved. |
| **Cryptography** | Is customer financial data encrypted both at rest (AES-256) and in transit (TLS 1.3)? | Yes | PCI-DSS v4.0 Req 4.2 / NIST PR.DS-01 | **COMPLIANT:** Vendor provided valid TLS configurations. No further action needed. |
| **Incident Response** | Do you guarantee customer notification within 72 hours of a confirmed data breach? | No | NIST IR.RP-01 / GDPR Art. 33 | **LEGAL GAP:** Reject contract terms. Amend the Service Level Agreement (SLA) to enforce the 72-hour limit. |



GRC Analyst Assessment Summary & Sign-Off

* **Vendor Evaluated:** PayGate API (Tier 1 - Critical)
* **Assessment Date:** 15 July 2026
* **Overall Assessment Status:** 🟡 Conditional Approval (Pending Remediation)

#### Analyst Final Recommendation:
PayGate API provides crucial credit card processing capabilities for our platform. However, the pre-onboarding security assessment revealed **two critical gaps**: a lack of enforced corporate MFA and non-compliant data breach notification timelines (7 days instead of the required 72 hours). 

To balance business enablement with operational risk mitigation, the GRC team issues a **Conditional Approval** based on the following mandatory remediation actions:
1. **MFA Enrolment**: PayGate must provide proof of enforced Multi-Factor Authentication configuration for all production environment administrators within 30 days.
2. **SLA Amendment**: Legal must update the vendor Master Services Agreement (MSA) to legally mandate a 72-hour breach notification timeline prior to contract signing.

**Analyst Signature:** [Nthabeleng Thebehadi], GRC Analyst Trainee
