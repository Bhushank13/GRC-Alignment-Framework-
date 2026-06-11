# Enterprise Access Control Policy

**Document Owner:** Chief Information Security Officer (CISO)  
**Effective Date:** January 15, 2025  
**Version:** 1.0  
**Framework Alignment:** ISO/IEC 27001:2022 (Control A.5.15), NIST CSF (PR.AC)

---

## 1. Purpose
The purpose of this policy is to establish the rules and requirements for granting, managing, and revoking logical access to enterprise information systems. This policy ensures that sensitive enterprise and customer data is protected from unauthorized access, modification, or disclosure.

## 2. Scope
This policy applies to all employees, contractors, third-party vendors, and system accounts (APIs/service accounts) that require access to the corporate network, cloud infrastructure, applications, or sensitive data.

## 3. Core Policy Directives

### 3.1 Principle of Least Privilege (PoLP) and Role-Based Access (RBAC)
*   Access to information systems shall be granted strictly based on the Principle of Least Privilege. Users will only receive the minimum level of access required to perform their authorized job duties.
*   Access rights must be tied to defined organizational roles (RBAC) rather than individual user preferences.
*   The use of shared or generic user accounts is strictly prohibited unless explicitly authorized by the CISO for specific system operations.

### 3.2 Authentication & Passwords
*   **Multi-Factor Authentication (MFA):** MFA is strictly mandated for all external, remote, and administrative access to corporate systems, including VPNs and cloud service consoles.
*   **Password Complexity:** Passwords must be a minimum of 14 characters in length and include a combination of uppercase, lowercase, numeric, and special characters.
*   **Lockout Threshold:** Accounts shall be automatically locked for a minimum of 30 minutes after 5 consecutive failed login attempts.

### 3.3 Privileged Access Management (PAM)
*   Standard end-users shall not be granted local administrative rights on corporate workstations.
*   IT and Security personnel requiring administrative access to servers or cloud environments must use dedicated, separate privileged accounts (e.g., `admin_jdoe`) and log in through a secure jump server or PAM solution.

### 3.4 Access Provisioning and Offboarding
*   **Onboarding:** All access requests must be formally submitted through the IT Service Management (ITSM) portal and approved by the user's direct manager and the respective Data Owner.
*   **Offboarding:** Upon employee or contractor termination, the HR department must notify IT immediately. All logical access must be completely revoked within 24 hours of the termination date.

### 3.5 User Access Reviews (UAR)
*   The GRC team shall coordinate mandatory User Access Reviews on a quarterly basis for critical systems (e.g., Financial databases, Cloud root accounts) and bi-annually for all other enterprise applications.
*   Data Owners must review and certify the access lists. Unjustified or dormant access must be revoked within 5 business days of the review.

## 4. Enforcement and Exceptions
Violations of this policy may result in disciplinary action, up to and including termination of employment or vendor contract termination. Any exceptions to this policy must be documented, justified by business need, and formally signed off by the Information Security department.