# Vendor Security Questionnaire (VSQ) & Risk Scoring Matrix

**Objective:** To assess the information security posture and regulatory compliance of third-party vendors handling sensitive enterprise data.

## 📊 Risk Scoring Methodology
Vendor responses are scored based on the criticality of the control. A "No" answer to a Critical control automatically flags the vendor for a mandatory mitigation review before onboarding.
*   **Critical Risk (Red):** Vendor lacks baseline compliance or encryption. (Auto-flag for executive review).
*   **High Risk (Orange):** Vendor lacks active monitoring or automated enforcement. (Requires remediation plan).
*   **Medium Risk (Yellow):** Missing formalized documentation, but compensating controls exist.
*   **Low Risk (Green):** Fully compliant with enterprise security standards.

---

## Section 1: Governance, Risk, and Compliance (GRC)

| ID | Security Question | Risk Weight | Yes/No | Vendor Comments / Compensating Controls |
| :--- | :--- | :--- | :--- | :--- |
| **GRC-01** | Does your organization hold an active, independent third-party security certification (e.g., SOC 2 Type II, ISO 27001)? | Critical | | |
| **GRC-02** | Is there a formally designated Information Security Officer (CISO) or dedicated security team? | High | | |
| **GRC-03** | Do you conduct mandatory security awareness training for all employees upon hire and at least annually thereafter? | Medium | | |
| **GRC-04** | Do you mandate background checks for all employees and contractors with access to sensitive data? | High | | |

## Section 2: Data Security & Privacy

| ID | Security Question | Risk Weight | Yes/No | Vendor Comments / Compensating Controls |
| :--- | :--- | :--- | :--- | :--- |
| **DSP-01** | Is all enterprise and customer data encrypted at rest using industry-standard algorithms (e.g., AES-256)? | Critical | | |
| **DSP-02** | Is all data transmitted over external networks encrypted in transit using TLS 1.2 or higher? | Critical | | |
| **DSP-03** | Can you provide a documented Data Retention and Secure Disposal policy? | Medium | | |
| **DSP-04** | Do you have mechanisms in place to comply with data privacy regulations (e.g., GDPR Right to be Forgotten)? | High | | |

## Section 3: Identity & Access Management (IAM)

| ID | Security Question | Risk Weight | Yes/No | Vendor Comments / Compensating Controls |
| :--- | :--- | :--- | :--- | :--- |
| **IAM-01** | Is Multi-Factor Authentication (MFA) strictly enforced for all remote access and administrative portals? | Critical | | |
| **IAM-02** | Is access to sensitive environments granted based on the Principle of Least Privilege and Role-Based Access Control (RBAC)? | High | | |
| **IAM-03** | Do you have an automated process to revoke access for terminated employees within 24 hours? | High | | |
| **IAM-04** | Do you support SAML/SSO integration for enterprise tenant access? | Low | | |

## Section 4: Vulnerability Management & AppSec

| ID | Security Question | Risk Weight | Yes/No | Vendor Comments / Compensating Controls |
| :--- | :--- | :--- | :--- | :--- |
| **VMA-01** | Do you conduct independent, third-party network and application penetration tests at least annually? | Critical | | |
| **VMA-02** | Is there a defined Service Level Agreement (SLA) ensuring critical vulnerabilities are patched within 7 to 14 days? | High | | |
| **VMA-03** | Do you integrate automated Static/Dynamic Application Security Testing (SAST/DAST) in your CI/CD pipeline? | Medium | | |
| **VMA-04** | Do you maintain a Software Bill of Materials (SBOM) to track open-source vulnerabilities? | High | | |

## Section 5: Incident Response & Business Continuity

| ID | Security Question | Risk Weight | Yes/No | Vendor Comments / Compensating Controls |
| :--- | :--- | :--- | :--- | :--- |
| **IRB-01** | Do you have a formally documented Incident Response Plan (IRP) that is tested at least annually? | Critical | | |
| **IRB-02** | Will our organization be notified of a confirmed security breach affecting our data within 48 hours? | Critical | | |
| **IRB-03** | Are immutable, offline backups maintained and tested quarterly to protect against ransomware? | High | | |
| **IRB-04** | Is a Disaster Recovery (DR) plan in place that guarantees a defined Recovery Time Objective (RTO)? | Medium | | |