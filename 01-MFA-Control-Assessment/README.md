# MFA Security Control Assessment

**Framework:** NIST SP 800-53 IA-2  
**Type:** Practice project using a fictional scenario  
**Status:** Completed written assessment

## Why I Chose This Project

I wanted to practice evaluating a security control from a GRC perspective instead of only looking at the technical side of cybersecurity.

I chose multi-factor authentication (MFA) because I have some experience supporting account access and authentication. However, I am still learning how to assess controls, document findings, and explain risk.

## The Scenario

For this exercise, I reviewed a fictional company that requires MFA for all employee accounts.

The scenario included two accounts with higher privileges that did not have MFA enabled. The company's policy did not allow exceptions.

My goal was to identify the control issue, determine the potential risk, and recommend how the company should address it.

## What I Found

**Control reviewed:** NIST SP 800-53 IA-2 — Identification and Authentication

**Finding:** Two privileged accounts did not have MFA enabled.

**My assessment:** The MFA requirement was not fully met.

I considered this a security concern because privileged accounts can make changes or access information that regular accounts cannot. If someone obtained the password for one of these accounts, the lack of MFA could make unauthorized access easier.

I would also want to understand why these accounts were not configured correctly and whether other accounts had the same problem.

## Evidence Reviewed

Because this is a fictional scenario, I worked with the following assumed information:

- The company has a policy requiring MFA for every employee.
- Two privileged accounts were identified without MFA.
- No exceptions to the policy were allowed.

For a real assessment, I would need to review account settings, access permissions, MFA configuration reports, and any relevant exception records.

I did not have actual system logs or configuration screenshots for this exercise.

## My Risk Assessment

I used a 5×5 risk matrix to practice evaluating likelihood and impact.

| Category | Rating |
| --- | --- |
| Likelihood | 4/5 |
| Impact | 4/5 |
| Risk score | 16/25 |
| Risk level | High |

### Why I Selected Likelihood 4/5

I selected 4 because two accounts with elevated permissions were missing MFA. If their passwords were compromised, an attacker might be able to access those accounts without completing a second authentication step.

I recognize that I would need more information about the accounts, their exposure, and existing security measures before confirming this rating in a real assessment.

### Why I Selected Impact 4/5

I selected 4 because unauthorized access to a privileged account could result in changes to systems, exposure of sensitive information, or disruption of operations.

The actual impact would depend on the permissions assigned to the accounts and the systems they could access.

### Overall Risk

4 × 4 = **16/25 — High**

For this exercise, I used a sample risk scale where scores from 15 to 19 are considered High. A real organization may use a different risk matrix.

## My Recommended Actions

If I were supporting the security team, I would recommend:

1. Notify the IT or security team about the two accounts.
2. Confirm whether the accounts still require privileged access.
3. Enable MFA for both accounts according to company policy.
4. Investigate why MFA was not enabled.
5. Review other privileged accounts to check for similar issues.
6. Document the corrective actions and verify that MFA is working.

I would also recommend reviewing the account onboarding process to help prevent the same issue from happening again.

## How I Would Verify the Issue Was Fixed

After the IT team completed the changes, I would want to confirm that MFA was enabled for both accounts and that the required authentication process worked correctly.

I would also request updated configuration evidence and document the results before recommending that the finding be closed.

**Retesting was not performed because this is a simulated exercise.**

## What I Learned

This exercise helped me understand that identifying a security issue is only one part of GRC work.

I also need to explain why the issue matters, determine the potential risk, recommend corrective actions, and identify what evidence would be needed to confirm that the problem was resolved.

One area I still want to improve is risk scoring. I understand how to calculate likelihood and impact, but I want more practice justifying those ratings using evidence rather than assumptions.

This project is part of my preparation for transitioning from technical cybersecurity work into Governance, Risk, and Compliance.

## Disclaimer

This is an educational project based on a fictional company. It does not include information from my employer or any real client.
