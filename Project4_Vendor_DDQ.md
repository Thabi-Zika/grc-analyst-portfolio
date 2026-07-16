# PROJECT 4: VENDOR DUE DILIGENCE QUESTIONNAIRE (DDQ)

1. Instruction & Scope
This Due Diligence Questionnaire (DDQ) must be completed by all external technology service providers prior to contract execution. Vendors must provide truthful answers and attach mandatory supporting evidence as requested. 

* Target Scope: Cloud Hosting, Core API Integrations, and Fleet Logistics Software Providers.
* Reviewing Frameworks: ISO/IEC 27001:2022 (A.5.19), NIST CSF v2.0 (GV.SC), COBIT 2019 (APO10)



2. Due Diligence Evaluation Table

| Assessment Domain | Due Diligence Question | Vendor Response (Yes/No) | Mandatory Evidence Required | GRC Analyst Validation Notes |
| :--- | :--- | :--- | :--- | :--- |
| **Security Governance** | Does your organisation maintain a formally approved Information Security Management System (ISMS)? | Yes | Copy of current ISO 27001 Certificate or recent SOC 2 Type II Report. | **VALIDATED:** ISO 27001 certificate verified against official registrar. Expiry date valid until December 2027. |
| **HR Security** | Are background checks and criminal record screenings performed on all employees with database access? | Yes | Anonymised sample of a completed employee background check report. | **VALIDATED:** Sample report reviewed. Confirms background verification processes match our internal standards. |
| **Data Management** | Do you utilise certified data destruction methods when decommissioning hardware containing client data? | No | Data Destruction Policy or sample Certificate of Destruction. | **CRITICAL GAP:** Vendor deletes data but does not use certified sanitisation methods (NIST SP 800-88). Remediation required. |
| **Business Continuity** | Are data backups replicated across geographically separate locations to survive a major regional outage? | Yes | Architecture diagram showing multi-region backup replication zones. | **VALIDATED:** AWS multi-region infrastructure diagram reviewed. Redundancy confirmed active. |



3. GRC Pre-Onboarding Governance Sign-Off

* Vendor Name: LogiCloud Solutions Ltd.
* Review Date: 16 July 2026
* Overall Determination: Onboarding Paused (Pending Evidence Remediation)

### Validation Summary:
While the vendor demonstrated acceptable maturity across Security Governance, HR Screenings, and AWS Cloud Infrastructure Redundancy, a critical compliance gap was identified in Data Management. The vendor cannot provide third-party verification or certified asset destruction records under NIST SP 800-88 guidelines. Onboarding is officially paused. The vendor must submit an updated hardware decommissioning addendum detailing certified data erasure mechanisms before contract negotiations can resume.

**Assessing Analyst:** [Nthabeleng Thebehadi], GRC Analyst Trainee
