# AI Governance & Agentic AI Audit Portfolio

## Aviation MRO Case Study

**Author:** Paweł Stuhldreer  
**Project Status:** Completed — Educational Proof of Concept (v1.0)  
**Industry:** Aviation Maintenance, Repair and Overhaul (MRO)  
**Technology:** Python 3, Google Colab, Jupyter Notebook

---

## 1. Project Overview

This independent portfolio project demonstrates the practical application of AI governance, risk management, internal controls and audit testing to a simulated AI agent supporting aviation Maintenance, Repair and Overhaul (MRO) activities.

The project focuses on the governance and control mechanisms necessary to support accountable, traceable and appropriately authorized AI-assisted workflows in a safety-critical industry.

It combines governance documentation, risk assessment, control design, a Python-based prototype and structured audit testing.

**The system is a demonstration prototype and is not intended for operational aviation use.**

## 2. Project Objectives

The primary objectives are to:

- Demonstrate a structured AI governance and risk management approach.
- Identify risks associated with AI-assisted MRO workflows.
- Design preventive and detective internal controls.
- Evaluate agent identity, authorization and delegation mechanisms.
- Demonstrate human oversight and approval requirements.
- Implement basic audit logging and traceability controls.
- Test the integrity of audit evidence.
- Document testing results, limitations and opportunities for improvement.

## 3. Governance and Regulatory References

The project draws on the following frameworks and references:

| Framework | Application |
|---|---|
| ISO/IEC 42001:2023 | AI management system governance and control design |
| Regulation (EU) 2024/1689 — EU AI Act | Regulatory applicability considerations |
| NIST AI RMF 1.0 | AI risk identification, assessment and management |
| OWASP AI security resources | Agentic AI security, authorization and accountability |
| NIST SP 800-92 | Security log management principles |

These references inform the project methodology. Their inclusion does not constitute certification, regulatory compliance verification or a formal conformity assessment.

## 4. Demonstration System

The prototype simulates an AI-assisted maintenance report analysis workflow.

A synthetic maintenance report is submitted for analysis. The demonstration system processes the report, applies predefined classification rules and produces a structured recommendation.

The workflow incorporates selected governance and security controls, including:

- Role-based authorization checks.
- Human approval requirements.
- Agent identity and delegation validation.
- Audit event recording.
- Hash-linked audit trail integrity verification.

The prototype uses deterministic Python logic rather than a deployed large language model.

No real aircraft maintenance records, operational systems or confidential organizational data are required.

## 5. Risk Management and Internal Controls

The project addresses selected governance and security risks, including:

- Unauthorized access to AI-assisted workflows.
- Execution of actions without required human approval.
- Misuse of agent permissions.
- Invalid or expired delegation.
- Insufficient accountability and traceability.
- Unauthorized modification of audit records.

Controls are designed and documented through a structured risk assessment and control matrix.

## 6. Audit Testing

The project includes a sequence of eight prototype test stages (TEST-01 to TEST-08), documented in the audit testing materials.

Selected verified demonstrations include:

### TEST-06 — Human Oversight Controls

Tests the simulated approval workflow, including prevention of execution before approval, rejection of unauthorized approval and recording of an authorized approval decision.

**Observed result:** PASS.

### TEST-07 — Agent Identity and Delegation Controls

Tests authorization behavior for recognized agents, unknown agents, unauthorized actions and expired delegations.

**Observed result:** PASS — 4/4 scenarios.

### TEST-08 — Audit Trail Integrity

Tests a SHA-256 hash-linked audit log against:

- Modification of an existing event.
- Deletion of an intermediate event.
- Reordering of recorded events.

**Observed result:** PASS — 4/4 scenarios.

The results demonstrate that the prototype passed the defined test assertions. They do not establish production-grade security or comprehensive compliance.

## 7. Repository Structure

| File | Description |
|---|---|
| `README.md` | Project overview and methodology |
| `01-AI-System-Description.md` | Simulated system description |
| `02-AI-Risk-Assessment.md` | Preliminary AI risk assessment |
| `03-AI-Control-Matrix.md` | Governance and internal control documentation |
| `04-Audit-Test-Results.md` | Test scenarios, results and evidence |
| `MRO_AI_Agent_Prototype.ipynb` | Python demonstration prototype |

## 8. Limitations

This project is an educational Proof of Concept.

It does not implement production-grade authentication, cryptographic agent identity verification, independently protected audit logs or comprehensive delegation-chain validation.

The hash-linked audit log demonstrates detection of selected modifications but does not provide full tamper resistance. Additional mechanisms, including trusted checkpoints and protected log storage, would be necessary for operational use.

The prototype has not undergone independent penetration testing, external certification or formal regulatory conformity assessment.

No operational aircraft maintenance or airworthiness decisions are performed.

## 9. Project Outcome

The project demonstrates the ability to translate AI governance and risk management concepts into practical control requirements, executable test scenarios and documented audit evidence.

It illustrates an integrated approach combining:

**Governance → Risk Assessment → Control Design → Technical Testing → Audit Evidence**

The completed Proof of Concept provides a foundation for further development of AI governance, agentic AI security and internal audit capabilities.

## 10. Author

**Paweł Stuhldreer**

Professional focus:

AI Governance | AI Risk Management | AI Compliance | AI Auditing | Internal Controls | Agentic AI Security

Areas of professional interest include ISO/IEC 42001, EU AI Act governance, AI management systems, audit evidence, human accountability and agent authorization controls.

---

## Disclaimer

This is an independent educational portfolio project developed using fictional scenarios and synthetic data.

It is not an official OWASP project, a certified AI management system or an audit of any real aviation organization.

References to industry standards and security frameworks are provided for educational and methodological purposes.

**Version:** 1.0  
**Date:** October 2026  
**Status:** Completed Educational Proof of Concept
