# PROJECT 2: FINTECH PAYMENT GATEWAY RISK REGISTER

1. Project Context
* **Target Industry:** FinTech (E-Commerce Payment Processing, Digital Wallets)
* **Framework Mapping:** PCI-DSS v4.0, NIST CSF v2.0 (Risk Assessment - Risk.ID)
* **Scenario:** An internal operational risk assessment of an online payment processing application handling high-frequency cardholder data to identify infrastructure and code vulnerabilities.



2. Risk Evaluation Methodology
To assess internal security threats objectively, we calculate an overall Risk Score by multiplying the likelihood of occurrence by the business impact:

**Risk Score = Likelihood (1 to 5) × Impact (1 to 5)**

*   **Score 1 to 6** = Low Risk (Acceptable, monitored annually)
*   **Score 8 to 12** = Medium Risk (Requires mitigation tracking within 90 days)
*   **Score 15 to 25** = High Risk (Immediate remediation required; executive escalation)



3. Active Risk Register Table

| Risk ID | Risk Description | Framework Mapping | Initial Score (L × I) | Mitigation Controls (The Plan) | Residual Score (L × I) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **RISK-01** | SQL Injection on checkout page allows malicious actors to steal customer financial data. | PCI-DSS v4.0 Req 6.2.4 | 15 <br>(Likelihood: 3 × Impact: 5) | Implement input validation, parameterised queries, and a Web Application Firewall (WAF). | 5 <br>(Likelihood: 1 × Impact: 5) |
| **RISK-02** | Developers accidentally commit plaintext API gateway keys to public GitHub repositories. | NIST CSF v2.0 PR.IR-02 | 16 <br>(Likelihood: 4 × Impact: 4) | Integrate automated secret-scanning tools (e.g. GitGuardian) into the CI/CD pipeline. | 4 <br>(Likelihood: 1 × Impact: 4) |
| **RISK-03** | Ransomware encrypts cross-border logistics tracking and freight dispatch databases. | ISO 27001:2022 A.8.14 | 12 <br>(Likelihood: 3 × Impact: 4) | Enforce hourly air-gapped backups and run quarterly disaster recovery simulation exercises. | 4 <br>(Likelihood: 2 × Impact: 2) |




4. GRC Risk Management Sign-Off

* **Review Date:** 16 July 2026
* **Next Review Cycle:** October 2026 (Quarterly)

### Executive Summary:
This assessment identified two High-Risk threats (SQL Injection and API Key leaks) capable of causing catastrophic financial and reputational damage. By applying target mitigation controls—specifically parameterised code, automated secret scanning, and hourly air-gapped backups—the residual risk across all domains has been successfully lowered to an acceptable level (Low). Continuous monitoring of compliance controls will be maintained via the automated CI/CD pipeline.

**Analyst Signature:** [Nthabeleng Thebehadi], GRC Analyst Trainee
