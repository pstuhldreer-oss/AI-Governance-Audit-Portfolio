# AI Risk Assessment

## 1. Document Information

**System:** MRO Maintenance Support Agent  
**Author:** Paweł Stuhldreer  
**Version:** 0.1  
**Status:** Preliminary assessment – pending validation

## 2. Purpose

This document identifies and evaluates preliminary AI-related risks associated with a simulated agent supporting administrative analysis of fictional aviation maintenance reports.

The assessment covers information security, AI reliability, access control, human oversight and accountability.

## 3. Risk Assessment Methodology

Risk Score = Probability (P) × Severity (S)

Probability:
1 – Rare
2 – Unlikely
3 – Possible
4 – Likely
5 – Almost certain

Severity:
1 – Negligible
2 – Minor
3 – Moderate
4 – Major
5 – Critical

Risk classification:
1–4: Low
5–9: Moderate
10–16: High
17–25: Critical

These scales and thresholds are project-specific assumptions and are not prescribed by ISO/IEC 42001.

## 4. Preliminary Risk Register

| ID | Risk | P | S | Score | Classification |
|---|---|---|---|---|---|
| AI-01 | AI hallucinations | 4 | 4 | 16 | High |
| AI-02 | Prompt injection | 4 | 4 | 16 | High |
| AI-03 | Unauthorized document access | 3 | 5 | 15 | High |
| AI-04 | Excessive agent permissions | 3 | 5 | 15 | High |
| AI-05 | Incomplete audit logging | 4 | 3 | 12 | High |
| AI-06 | Outdated reference information | 4 | 4 | 16 | High |
| AI-07 | Ineffective human oversight | 3 | 5 | 15 | High |
| AI-08 | Sensitive information disclosure | 3 | 4 | 12 | High |

## 5. Proposed Risk Treatment Measures

### AI-01 – Hallucinations
Control: Source-grounded responses, uncertainty indicators and mandatory human review.

### AI-02 – Prompt Injection
Control: Input validation, separation of instructions and retrieved content, and adversarial testing.

### AI-03 – Unauthorized Access
Control: Role-based access control and document-level authorization.

### AI-04 – Excessive Permissions
Control: Least privilege, tool allowlists and explicit approval for sensitive actions.

### AI-05 – Incomplete Logging
Control: Structured event logging, unique request identifiers and audit trail verification.

### AI-06 – Outdated Information
Control: Source versioning, validity metadata and freshness checks.

### AI-07 – Human Oversight Failure
Control: Mandatory approval checkpoints, reviewer training and escalation procedures.

### AI-08 – Information Disclosure
Control: Synthetic test data, data minimization and output filtering.

## 6. Risk Treatment Status

All controls are proposed and have not yet been verified.

Residual risk: Not assessed.

Risk acceptance: Pending documented review.

## 7. Next Steps

1. Define risk owners and acceptance criteria.
2. Identify existing and proposed controls.
3. Develop test cases for each control.
4. Implement the simulated agent.
5. Collect evidence of control effectiveness.
6. Reassess residual risks.
7. Document formal risk treatment decisions.

## 8. References

- ISO/IEC 42001:2023
- ISO/IEC 23894:2023
- NIST AI Risk Management Framework
- OWASP AI Security and Privacy Guide
- Regulation (EU) 2024/1689

## 9. Disclaimer

This is an educational risk assessment based on a fictional AI system. The risk ratings are illustrative assumptions and do not represent measured operational risk in an aviation maintenance organization.
