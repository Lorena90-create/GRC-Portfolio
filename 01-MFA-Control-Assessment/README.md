# MFA Security Control Assessment

**Framework:** NIST SP 800-53 IA-2 — Identification and Authentication  
**Project Type:** Educational Simulation  
**Status:** Written assessment completed

## 1. Purpose

The purpose of this project is to practice evaluating a cybersecurity control using basic Governance, Risk, and Compliance (GRC) principles.

Multi-factor authentication (MFA) was selected because it is an important security measure for protecting user accounts and preventing unauthorized access.

The assessment focuses on identifying a control weakness, evaluating the associated risk, and recommending corrective actions.

## 2. Scenario

A fictional organization has a security policy requiring MFA for all employee accounts, without exceptions.

During a simulated review, two privileged accounts were identified without MFA enabled.

These accounts have elevated permissions, making the missing authentication requirement a potential security concern.

## 3. Control Assessment

**Control:** NIST SP 800-53 IA-2 — Identification and Authentication

**Finding:** Two privileged accounts do not have MFA enabled.

**Assessment Result:** The organization's MFA requirement is not fully met.

The finding represents a security weakness because privileged accounts may provide access to sensitive information or critical system settings.

Without MFA, compromised credentials could potentially be used to gain unauthorized access.

## 4. Evidence Considered

The assessment is based on the following fictional information:

- Organizational policy requires MFA for all employees.
- Two privileged accounts have MFA disabled.
- No policy exceptions are permitted.

In a real assessment, additional evidence would be needed, including MFA configuration reports, user permissions, and relevant authentication records.

No actual system testing was performed.

## 5. Risk Assessment

A 5×5 risk matrix was used to estimate the potential likelihood and impact of the finding.

| Risk Factor | Rating |
| --- | --- |
| Likelihood | 4/5 — Likely |
| Impact | 4/5 — Major |
| Risk Score | 16/25 |
| Overall Risk | High |

### Likelihood Justification

A likelihood rating of 4/5 was selected because two privileged accounts lack MFA protection.

This increases exposure to credential-based attacks, particularly if account passwords are compromised.

The rating is preliminary because account exposure, threat activity, and other security controls have not been verified.

### Impact Justification

An impact rating of 4/5 was selected because unauthorized access to privileged accounts could result in system changes, exposure of sensitive information, or interruption of operations.

The actual impact would depend on the accounts' permissions and the systems they can access.

### Overall Risk Rating

**4 × 4 = 16/25 — High**

For this educational exercise, scores between 15 and 19 are classified as High. Actual organizational risk ratings depend on the approved risk assessment methodology.

## 6. Recommended Remediation

The following actions are recommended:

1. Notify the IT security team of the finding.
2. Verify the affected accounts and their assigned privileges.
3. Enable MFA for both accounts according to organizational policy.
4. Investigate why MFA was not enabled.
5. Review other privileged accounts for similar configuration issues.
6. Update account provisioning procedures to reduce the possibility of recurrence.

## 7. Verification and Follow-Up

After remediation, the IT security team should verify that MFA is enabled and functioning correctly for both accounts.

Updated configuration records should be reviewed and documented as evidence of corrective action.

The finding should remain open until the required security control has been verified.

**Retesting Status:** Not performed — simulated assessment.

## 8. Lessons Learned

This exercise demonstrates that security control assessments involve more than identifying technical weaknesses.

An effective assessment also requires documenting findings, evaluating potential risks, recommending remediation, and determining how corrective actions will be verified.

Additional practice is needed in evidence collection, risk scoring, and formal control testing to develop stronger GRC assessment skills.

## Disclaimer

This project is an educational simulation based on a fictional organization. No real employer, client, or government information was used.
