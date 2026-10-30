# Cybersecurity Risk Register

**Reference:** NIST SP 800-30 Rev. 1 — Guide for Conducting Risk Assessments  
**Project Type:** Educational simulation  
**Status:** Completed — Educational Simulation

## 1. Purpose

This project demonstrates how a basic risk register can be used to document and prioritize cybersecurity risks.

A risk register helps organizations keep track of identified risks, their potential impact, recommended actions, and the teams responsible for addressing them.

## 2. Scenario

A fictional company with approximately 150 employees uses cloud applications, Windows workstations, and an internal network to support daily operations.

During a simulated security review, five potential weaknesses were identified. The purpose of the exercise is to assess the possible risks and recommend corrective actions.

No actual systems or company records were reviewed.

## 3. Risk Assessment Method

A 5×5 matrix was used to estimate likelihood and impact.

Likelihood represents how likely a security event is to occur and cause harm. Impact represents the potential consequences for the organization.

Risk Score = Likelihood × Impact

### Scoring Scale

| Score | Description |
| --- | --- |
| 1–4 | Low |
| 5–9 | Moderate |
| 10–14 | Elevated |
| 15–19 | High |
| 20–25 | Critical |

This is a sample scoring method created for the exercise. Organizations may use different risk rating criteria.

## 4. Risk Register

| ID | Identified Risk | Likelihood | Impact | Score | Rating |
| --- | --- | --- | --- | --- | --- |
| R-001 | Privileged accounts without MFA | 4 | 4 | 16 | High |
| R-002 | Unsupported operating systems | 4 | 3 | 12 | Elevated |
| R-003 | Backup restoration not tested | 3 | 5 | 15 | High |
| R-004 | Delayed critical vulnerability remediation | 4 | 4 | 16 | High |
| R-005 | Excessive user access permissions | 3 | 4 | 12 | Elevated |

## 5. Risk Evaluation and Recommended Actions

### R-001: Privileged Accounts Without MFA

**Risk:** Two privileged accounts do not have multi-factor authentication enabled.

**Likelihood — 4/5:** Missing MFA increases the possibility of unauthorized access if account credentials are compromised.

**Impact — 4/5:** Compromise of privileged accounts could allow unauthorized system changes or access to sensitive information.

**Recommended Action:** Enable MFA, verify the affected accounts, and review MFA enforcement for other privileged users.

**Suggested Owner:** Identity and Access Management Team

### R-002: Unsupported Operating Systems

**Risk:** Several workstations are running operating systems that no longer receive regular security updates.

**Likelihood — 4/5:** Known vulnerabilities may remain unpatched, increasing the possibility of exploitation.

**Impact — 3/5:** A compromised workstation could expose company information or interrupt employee productivity. Broader impact depends on network access and existing protections.

**Recommended Action:** Identify affected devices, upgrade or replace unsupported systems, and apply temporary security restrictions where needed.

**Suggested Owner:** IT Operations Team

### R-003: Backup Restoration Not Tested

**Risk:** Backups are performed regularly, but the company has not tested whether important systems can be restored successfully.

**Likelihood — 3/5:** A restoration failure is possible because backup recovery procedures have not been verified.

**Impact — 5/5:** If critical systems cannot be restored after an outage or ransomware incident, the company could experience significant operational disruption and data loss.

**Recommended Action:** Schedule restoration tests, document the results, and correct any identified recovery problems.

**Suggested Owner:** IT Infrastructure Team

### R-004: Delayed Vulnerability Remediation

**Risk:** Several critical vulnerabilities remain unresolved beyond the company's remediation deadline.

**Likelihood — 4/5:** Systems with unresolved critical vulnerabilities may be exposed to known attack methods. Actual likelihood depends on exposure and available security controls.

**Impact — 4/5:** Successful exploitation could affect system availability, confidentiality, or integrity.

**Recommended Action:** Prioritize remediation based on severity, exposure, and business importance. Track corrective actions until verification is completed.

**Suggested Owner:** Vulnerability Management and IT Teams

### R-005: Excessive User Access Permissions

**Risk:** Some employees retain access to systems that are no longer required for their current responsibilities.

**Likelihood — 3/5:** Unnecessary permissions increase the opportunity for misuse or unauthorized access, although no misuse is assumed in this scenario.

**Impact — 4/5:** Inappropriate access could result in unauthorized changes or exposure of sensitive information.

**Recommended Action:** Conduct periodic access reviews, remove unnecessary permissions, and verify that access matches job responsibilities.

**Suggested Owner:** IAM Team and Department Managers

## 6. Risk Prioritization

Based on the preliminary scores, risks R-001, R-003, and R-004 require the highest attention.

These risks involve privileged access, recovery capabilities, and unresolved critical vulnerabilities.

R-002 and R-005 should also be addressed, but their priority may change after additional evidence is reviewed.

Risk scores alone should not determine remediation order. Business criticality, system exposure, existing controls, and organizational requirements must also be considered.

## 7. Evidence Needed for a Real Assessment

Before confirming the ratings, the following information would be useful:

- MFA configuration and privileged account reports
- Operating system inventory and support status
- Backup restoration test records
- Vulnerability scan findings and remediation tickets
- User access review reports

The information in this exercise is fictional. No actual testing or evidence collection was performed.

## 8. Lessons Learned

A risk register provides a structured way to organize security concerns and communicate them to the responsible teams.

The exercise also highlights the importance of explaining risk ratings rather than assigning numbers without supporting information.

Additional practice is needed in reviewing evidence, determining likelihood, and evaluating how existing security controls affect risk.

## 9. Reference

NIST SP 800-30 Rev. 1 — Guide for Conducting Risk Assessments  
https://csrc.nist.gov/pubs/sp/800/30/r1/final

## Disclaimer

This project is an educational simulation involving a fictional organization. It does not represent an assessment of any actual employer, client, or government system.
