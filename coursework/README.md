# Cybersecurity Coursework

Selected coursework in risk assessment and web security. Reports are presented as PDFs, with CSV data or source code alongside them where applicable.

| Project | Focus | Reports | Data or code |
| --- | --- | --- | --- |
| Mojang Studios risk assessment | Asset identification, likelihood-impact scoring, and proposed risk treatments | [Read PDF](mojang-risk-assessment/data/Mojang%20Studios%20Risk%20Assessment.pdf) | Report-based project |
| Web security analysis and login lab | Web vulnerability analysis and an intentionally vulnerable local login application | [Read PDF](web-security-lab/reports/web-security-analysis.pdf) | [Lab and setup](web-security-lab/README.md) |
| Financial-services risk assessment | Anonymized analysis of phishing, vendor compromise, and ransomware scenarios | [Read PDF](financial-services-risk-assessment/reports/financial-services-risk-assessment.pdf) | Report-based project |
| S.O.F.T. financial threat model | Team-developed conceptual framework with explicit scoring, a hypothetical worked example, and trust boundaries | [Read PDF](soft-threat-model/reports/soft-threat-model.pdf) | [Diagram and sources](soft-threat-model/SOURCES.md); no deployed implementation claimed |

## S.O.F.T. — Student Organization Financial Threat Model

A team-developed conceptual model connecting financial-workflow threats to four stages: threat categorization, likelihood-impact assessment using a 4 × 4 matrix, risk triage, and targeted mitigation. It considers impersonation, excessive access, information interception or tampering, and transaction/accountability failures. Its scope is student-organization finances; broader company coverage and control effectiveness have not been validated. Team credit: Dhruv Guda and Owen Kedroski.

## References and scope

- Sources: [Mojang assessment](mojang-risk-assessment/SOURCES.md), [web security](web-security-lab/SOURCES.md), [financial-services assessment](financial-services-risk-assessment/SOURCES.md), [S.O.F.T.](soft-threat-model/SOURCES.md).
- See the assessment’s [method and limitations](mojang-risk-assessment/REVIEW-NOTES.md). Proposed controls and modeled scores are not demonstrated company outcomes.
- The financial-services assessment is anonymized; it makes no verified internal-control or breach claims about an identifiable organization.
- The login lab deliberately contains SQL injection and weak password hashing. Use only in an isolated, authorized local environment. Never enter real credentials or deploy publicly. Read [security guidance](SECURITY.md) and [third-party notices](THIRD-PARTY-NOTICES.md).
