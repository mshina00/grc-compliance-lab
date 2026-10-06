# Laws and Regulations Reference

> Educational summary, not legal advice. Dates, thresholds, and enforcement status change. **Verify against the official source** before citing. Last reviewed: 6 October 2026. See `REFERENCES.md` for official sources.

## United States

| Name | Full form | Applies to | Function / purpose | Key points |
|---|---|---|---|---|
| **HIPAA** | Health Insurance Portability and Accountability Act (1996) | Healthcare providers, health plans, clearinghouses ("covered entities") and their business associates | Protects the privacy and security of patient health information (PHI / ePHI) | Privacy Rule, Security Rule (administrative, physical, technical safeguards), Breach Notification Rule (notify individuals without unreasonable delay, no later than 60 days after discovery). Enforced by HHS Office for Civil Rights (OCR). Business Associate Agreements (BAAs) required. |
| **HITECH** | Health Information Technology for Economic and Clinical Health Act (2009) | Same as HIPAA | Strengthens HIPAA enforcement and breach notification; promotes electronic health records | Extends HIPAA directly to business associates; raises penalties. |
| **SOX** | Sarbanes-Oxley Act (2002) | US public companies and their auditors | Prevents financial reporting fraud; requires reliable internal controls | Section 302 (executive certification), Section 404 (internal control over financial reporting). IT General Controls (ITGC) such as access, change management, and operations are commonly tested. |
| **GLBA** | Gramm-Leach-Bliley Act (1999) | Financial institutions | Protects consumers' nonpublic personal financial information | Financial Privacy Rule, Safeguards Rule (written information security program), pretexting provisions. FTC and financial regulators enforce. |
| **FISMA** | Federal Information Security Modernization Act (2014) | US federal agencies and their contractors | Requires agencies to implement information security programs | Uses NIST standards (SP 800-53, RMF). Annual reporting and assessment. |
| **FedRAMP** | Federal Risk and Authorization Management Program | Cloud providers selling to US federal agencies | Standardized security assessment and authorization of cloud services | Based on NIST SP 800-53 baselines (Low, Moderate, High). Third-party assessment organizations (3PAOs) assess. |
| **CMMC** | Cybersecurity Maturity Model Certification | Defense Industrial Base contractors for the US Department of Defense | Verifies protection of Federal Contract Information (FCI) and Controlled Unclassified Information (CUI) | CMMC 2.0 has three levels; Level 2 aligns with NIST SP 800-171. Phased rollout began Nov 2025; industry reporting says the DoD suspended Phase 2 (mandatory third-party Level 2 assessments) in July 2026 pending review, while self-assessment requirements continue. Check the DoD CIO page. |
| **NYDFS 23 NYCRR 500** | New York Department of Financial Services Cybersecurity Regulation | Financial and insurance firms licensed in New York | Mandates cybersecurity programs for regulated entities | Requires a CISO, risk assessments, MFA, annual certification, and 72-hour notice of cybersecurity events. |
| **SEC Cyber Disclosure Rules** | US Securities and Exchange Commission cybersecurity disclosure rules (2023) | US public companies | Timely, consistent investor disclosure of cyber risk and incidents | Form 8-K Item 1.05 within four business days of determining an incident is material; annual risk management and governance disclosure in Form 10-K. |
| **CIRCIA** | Cyber Incident Reporting for Critical Infrastructure Act (2022) | Critical infrastructure entities | Mandatory incident reporting to CISA | 72 hours for covered incidents, 24 hours for ransom payments. Final rule not yet published as of October 2026; reported at White House review, with publication expected by year end. Check CISA. |
| **CCPA / CPRA** | California Consumer Privacy Act (2018) / California Privacy Rights Act (2020) | For-profit businesses meeting thresholds that handle California residents' data | Gives consumers rights over personal information | Rights to know, delete, correct, opt out of sale/sharing, limit use of sensitive data. Enforced by the California Privacy Protection Agency (CPPA) and Attorney General. |
| **FERPA** | Family Educational Rights and Privacy Act (1974) | Schools receiving US federal education funds | Protects student education records | Parent/student access and consent rules for disclosure. |
| **COPPA** | Children's Online Privacy Protection Act (1998) | Online services directed at children under 13 | Protects children's online personal information | Verifiable parental consent; FTC enforced. |

## European Union and United Kingdom

| Name | Full form | Applies to | Function / purpose | Key points |
|---|---|---|---|---|
| **GDPR** | General Data Protection Regulation (EU) 2016/679 | Any organization processing personal data of people in the EU/EEA | Protects personal data and privacy rights | Lawful basis, data subject rights (access, erasure, portability), DPIAs, DPO where required, 72-hour breach notification to the supervisory authority. Fines up to EUR 20 million or 4% of global annual turnover, whichever is higher. |
| **UK GDPR + DPA 2018** | United Kingdom General Data Protection Regulation and Data Protection Act 2018 | Organizations processing UK residents' data | UK version of GDPR after Brexit | Regulated by the Information Commissioner's Office (ICO). |
| **NIS2** | Network and Information Security Directive 2 (EU) 2022/2555 | Essential and important entities in sectors such as energy, health, transport, digital infrastructure | Raises the baseline of cybersecurity across the EU | Risk management measures, supply chain security, management accountability. Early warning within 24 hours, incident notification within 72 hours, final report within one month. Applied through national laws. |
| **DORA** | Digital Operational Resilience Act (EU) 2022/2554 | EU financial entities and their critical ICT third-party providers | Ensures the financial sector can withstand ICT disruption | ICT risk management, incident reporting, resilience testing, third-party risk oversight. Applies since 17 January 2025. |
| **EU AI Act** | Regulation (EU) 2024/1689 on Artificial Intelligence | Providers and deployers of AI systems in the EU market | Risk-based regulation of AI | Prohibited, high-risk, limited-risk, and minimal-risk tiers. Prohibitions apply since Feb 2025 and general-purpose AI obligations since Aug 2025. Under the AI Omnibus, high-risk obligations are delayed to 2 Dec 2027 (stand-alone systems) and 2 Aug 2028 (embedded in products). |
| **CRA** | Cyber Resilience Act (EU) 2024/2847 | Manufacturers of products with digital elements sold in the EU | Security requirements across the product life cycle | Security by design, vulnerability handling, and reporting. Phased application. |

## Other Regions

| Name | Full form | Region | Function |
|---|---|---|---|
| **PIPEDA** | Personal Information Protection and Electronic Documents Act | Canada | Governs private-sector handling of personal information. |
| **LGPD** | Lei Geral de Proteção de Dados (General Data Protection Law) | Brazil | Brazil's comprehensive data protection law, similar to GDPR. |
| **DPDP Act** | Digital Personal Data Protection Act, 2023 | India | Governs processing of digital personal data; rules are being phased in. |
| **PDPA** | Personal Data Protection Act 2012 | Singapore | Governs collection, use, and disclosure of personal data. |
| **Privacy Act 1988** | Privacy Act 1988 (with Notifiable Data Breaches scheme) | Australia | Governs personal information handling and breach notification. |

## Quick comparison: breach notification clocks

| Regime | Clock (verify current text) |
|---|---|
| GDPR | 72 hours to regulator after becoming aware |
| NIS2 | 24 hours early warning, 72 hours notification |
| NYDFS 500 | 72 hours |
| CIRCIA | 72 hours (incident), 24 hours (ransom payment) |
| SEC | 4 business days after materiality determination |
| HIPAA | Without unreasonable delay, no later than 60 days |


---
© 2026 Hina Qurashee. All rights reserved.
