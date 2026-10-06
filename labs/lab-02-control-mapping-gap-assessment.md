# Lab 02: Control Mapping and Gap Assessment

**Time:** 3 hours | **Frameworks:** ISO 27001, NIST CSF 2.0, SOC 2, HIPAA, PCI DSS

## Objectives
- Map one control to multiple frameworks ("test once, comply many").
- Assess implementation status and identify gaps.
- Prioritize remediation.

## Reference mapping (illustrative; validate against current official texts)

| Control area | ISO 27001:2022 Annex A | NIST CSF 2.0 | NIST 800-53 | SOC 2 | PCI DSS v4.0 | HIPAA Security Rule |
|---|---|---|---|---|---|---|
| Multi-factor authentication | A.5.17, A.8.5 | PR.AA | IA-2 | CC6.1 | Req. 8.4 | 164.312(d) |
| Logging and monitoring | A.8.15, A.8.16 | DE.CM | AU-2, AU-6 | CC7.2 | Req. 10 | 164.312(b) |
| Backups | A.8.13 | PR.DS | CP-9 | A1.2 | Req. 12.10 (recovery in IR plan) | 164.308(a)(7)(ii)(A) |
| Incident response | A.5.24 - A.5.28 | RS.MA | IR-4 | CC7.3 - CC7.5 | Req. 12.10 | 164.308(a)(6) |
| Vulnerability management | A.8.8 | ID.RA | RA-5 | CC7.1 | Req. 6.3, 11.3 | 164.308(a)(1)(ii)(A) |
| Security awareness training | A.6.3 | PR.AT | AT-2 | CC1.4 | Req. 12.6 | 164.308(a)(5) |

## Tasks
1. Create `my-work/control-mapping.csv` with columns: Control, ISO, CSF, 800-53, SOC 2, PCI, HIPAA, Status, Evidence, Gap, Owner.
2. Add **6 more control areas** (for example: encryption, change management, vendor management, physical security, access reviews, secure development).
3. Set Status for each: *Implemented, Partial, Not Implemented, Not Applicable*.
4. For Partial and Not Implemented controls, write the gap and a remediation step.
5. Calculate the percentage implemented per framework.
6. Rank the top five gaps by risk and effort.

## Deliverables
- Completed mapping CSV.
- One-page gap summary with a prioritized remediation roadmap.

## Self-check
- Is each status backed by named evidence (a screenshot, config export, policy, ticket)?
- Are "Not Applicable" entries justified (needed for an ISO 27001 Statement of Applicability)?


---
© 2026 Hina Qurashee. All rights reserved.
