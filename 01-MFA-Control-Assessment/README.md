# MFA Security Control Assessment

**Framework:** NIST SP 800-53 — IA-2 (Identification and Authentication)  
**Project Type:** Educational simulation  
**Assessment Status:** Completed (simulation)

## 1. Objective

Evaluate the implementation of multi-factor authentication (MFA) for privileged user accounts, identify control weaknesses, assess associated risks, and recommend corrective actions.

## 2. Scenario

A fictional organization requires MFA for all employee accounts, with no exceptions. During a simulated access-control review, two accounts with elevated privileges were identified without MFA enabled.

The assessment focuses on this known policy violation. Additional evidence would be required to determine the full scope and cause.

## 3. Control Requirement

NIST SP 800-53 IA-2 addresses identification and authentication of organizational users. Relevant IA-2 enhancements address multi-factor authentication for privileged and non-privileged accounts.

**Organizational policy:** MFA must be enabled for all employee accounts without exceptions.

## 4. Assessment Approach and Evidence

**Assessment methods:** Examine configuration records, interview responsible personnel, and test authentication settings where authorized.

| Evidence | Simulated result |
| --- | --- |
| MFA policy | MFA required for all employee accounts |
| Account configuration review | Two privileged accounts have MFA disabled |
| Privilege review | Both affected accounts have elevated permissions |
| Approved exception records | No exceptions permitted by policy |

**Evidence limitations:** The scenario does not provide authentication logs, account exposure details, system criticality, or evidence of compromise. Those items would be requested during a real assessment.

## 5. Finding

**Finding ID:** MFA-001  
**Title:** MFA Not Enabled for Two Privileged Accounts  
**Control:** NIST SP 800-53 IA-2 and applicable MFA enhancements  
**Control effectiveness:** Not fully effective

Two privileged accounts do not have MFA enabled, contrary to the organization's policy. This weakness increases the risk that compromised credentials could be used to gain unauthorized privileged access.

## 6. Risk Assessment

**Method:** Qualitative 5×5 likelihood-impact matrix

| Factor | Score | Rationale |
| --- | --- | --- |
| Likelihood | 4/5 — Likely | Missing MFA increases exposure to credential-based attacks. The two affected accounts have elevated privileges. The rating is provisional because actual exposure and threat activity are unknown. |
| Impact | 4/5 — Major | Unauthorized use of privileged accounts could allow sensitive data access, unauthorized configuration changes, or service disruption. Actual impact depends on the accounts' permissions and accessible systems. |
| Overall risk | 16/25 — High | Likelihood 4 × Impact 4 = 16. This exercise defines 15–19 as High. |

### Risk rating scale used for this exercise

- 1–4: Low
- 5–9: Moderate
- 10–14: Elevated
- 15–19: High
- 20–25: Critical

**Preliminary risk rating: HIGH**

The rating is an educational judgment, not a measured probability or confirmed business impact. A real assessment would apply the organization's approved risk criteria.

## 7. Recommended Remediation

1. **Immediate containment:** Notify the security and IAM teams, verify the two accounts and their business need, and apply temporary restrictions if appropriate.
2. **Correct the finding:** Enable and verify MFA for both privileged accounts using organization-approved methods.
3. **Investigate root cause:** Review account provisioning, authentication policies, and configuration enforcement to determine why MFA was missing.
4. **Prevent recurrence:** Implement automated checks for MFA coverage and periodic reviews of privileged accounts.
5. **Document completion:** Record the changes, responsible personnel, verification results, and closure evidence.

**Suggested remediation owner:** Identity and Access Management (IAM) team, with security oversight.

**Suggested target:** Prioritize immediate review and establish a corrective-action deadline based on organizational policy and risk acceptance procedures.

## 8. Validation and Retesting

The assessor should verify that:

- MFA is enabled for both affected accounts.
- Each account successfully completes the approved MFA authentication flow.
- Privileged access is not granted when required MFA is missing.
- Configuration records or logs support the remediation.
- A broader review identifies any similar gaps.

**Closure criteria:** Both accounts meet the MFA requirement, evidence is retained, and the security team confirms the finding is resolved.

**Retest status:** Not performed — fictional scenario.

## 9. Lessons Learned

This exercise helped me practice identifying a control gap, distinguishing a policy violation from a risk rating, documenting evidence limitations, explaining likelihood and impact, and defining remediation and retesting steps.

In a real GRC assessment, I would seek additional evidence, validate assumptions with control owners, and follow the organization's risk assessment methodology before finalizing the rating.

## Disclaimer

This is an independent educational simulation using fictional information. It is not an assessment of any real employer, client, or government system. No confidential information is included.
