# Fortnight Report: Cybersecurity Research on UK Neobanks

| Field | Detail |
|---|---|
| Intern | Hina Qurashee |
| Position | Cybersecurity Intern |
| Organization | ABC Company |
| Period covered | 10 Oct - 24 Oct 2025 |

## Overview
Assessed the cybersecurity posture, compliance standards, and risk management practices of major UK-based neobanks. Goal: identify common vulnerabilities, analyze security frameworks, and recommend best practices for digital banking resilience.

## Key Research Activities
- Reviewed public security policies and compliance documentation of UK neobanks such as Monzo, Revolut, Starling Bank, and Atom Bank.
- Examined FCA (Financial Conduct Authority) and PRA (Prudential Regulation Authority) guidance relevant to cybersecurity and data protection.
- Analyzed customer data protection practices under GDPR and PSD2.
- Studied authentication mechanisms: multi-factor authentication, biometrics, and session management.
- Evaluated encryption standards for data in transit and at rest.
- Reviewed threat intelligence reports and common attack vectors (phishing, API vulnerabilities, insider threats).
- Used Wireshark for network traffic analysis (simulation).
- Reviewed penetration testing frameworks (OWASP, NIST).
- Reviewed NIST cybersecurity compliance guidance [confirm which: for example CSF 2.0, SP 800-53, SP 800-63B, SP 800-115, SP 800-207].
- Compared secure app architecture between traditional and digital-only banks.

## Findings
- Strong user-side encryption, but heavy reliance on third-party cloud providers introduces shared-responsibility risk.
- API security is a high-priority concern; improper access control and token handling recur in open banking APIs.
- Continuous SOC monitoring and threat intelligence integration need improvement.
- ISO/IEC 27001 and GDPR alignment is consistent, but incident response documentation varies between institutions.

*Findings are based on public references, public documentation, and threat intelligence research, not on testing of any organization's systems. Findings describe common industry patterns and are not attributed to any individual company.*

## NIST Alignment
| Finding / recommendation | Relevant NIST guidance |
|---|---|
| Third-party cloud and shared responsibility | NIST CSF 2.0 Govern (supply chain risk management), SP 800-53 SR family |
| API and authentication weaknesses | SP 800-63B (authentication), SP 800-53 IA and AC families |
| SOC monitoring and threat intelligence | CSF 2.0 Detect, SP 800-53 SI-4 and AU families |
| Incident response documentation | CSF 2.0 Respond, SP 800-61 (incident handling) |
| Zero Trust Architecture | SP 800-207 |
| Penetration testing | SP 800-115 |

*This table is my mapping of findings to NIST guidance, for reference.*

## Recommendations
- Strengthen third-party risk management and conduct periodic security audits.
- Improve API authentication and monitoring using token rotation and anomaly detection.
- Apply Zero Trust Architecture (ZTA) principles across all network layers.
- Increase security awareness training, especially for social engineering.
- Keep incident response playbooks current with frequent simulation drills.

## Next Steps
- Build a risk assessment matrix to score vulnerabilities across neobanks (see `artifacts/Sample_Risk_Register_GRC.xlsx` for the method).
- Prepare a comparative chart of regulatory compliance (FCA, GDPR, PSD2) (see `docs/neobank-regulations-uk-us.md`).
- Draft the final cybersecurity framework proposal for neobanks.

## Summary
The research shows how digital-first banks balance innovation with compliance while managing evolving security threats.


---
© 2026 Hina Qurashee. All rights reserved.
