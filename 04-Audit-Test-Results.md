# AI Governance – Initial Audit Test Results

**Project:** AI Governance & Agentic AI Audit Portfolio  
**System:** Simulated MRO Maintenance Support Agent  
**Auditor:** Paweł Stuhldreer  
**Test date:** 15 October 2026  
**Environment:** Google Colab / Python  
**Status:** Initial prototype testing

## 1. Audit Objective

To evaluate selected access control and audit logging mechanisms implemented in a simulated aviation MRO report-processing workflow.

## 2. Test Results

| Test ID | Control | Result | Evidence |
|---|---|---|---|
| TEST-03 | Role-based access decisions | PASS – 4/4 | Colab test output |
| TEST-03-INT | Access enforcement through secured wrapper | PASS – 5/5 | Colab integration test |
| TEST-05 | In-memory audit event recording | PASS | Four recorded events |

## 3. Key Findings

**Access Control:** Authorized roles were permitted to process simulated reports, while unauthorized and unknown roles were denied through the secured workflow.

**Audit Logging:** Four events were recorded, including two successful processing operations and two denied operations. Events included identifiers, timestamps, roles, actions and authorization outcomes.

**Human Oversight:** The initial workflow generates recommendations with a PENDING approval status. Approval enforcement has not yet been tested.

## 4. Limitations

- The prototype does not yet use a language model.
- Access control is implemented in a demonstration wrapper and can be bypassed through direct function calls.
- Audit logs are stored in memory and are not tamper-resistant.
- User identities are represented by supplied role strings rather than authenticated identities.
- Tests use synthetic data and a limited number of scenarios.
- No production aviation environment has been assessed.

## 5. Preliminary Conclusion

The prototype passed the defined functional tests for role-based access decisions, secured workflow execution and basic event logging.

These results provide initial evidence of control functionality but do not demonstrate production-level control effectiveness or regulatory compliance.

## 6. Next Steps

1. Implement structured and persistent audit logging.
2. Introduce authenticated identities and stronger authorization enforcement.
3. Test human approval checkpoints.
4. Add an LLM-based analysis component.
5. Conduct adversarial testing and document residual risks.

## 7. References

- ISO/IEC 42001:2023 – Artificial intelligence management systems.
- NIST SP 800-53 Rev. 5 – Security and Privacy Controls.
- NIST AI Risk Management Framework 1.0.
- OWASP guidance on AI and LLM security.


## TEST-07 – Agent Identity & Delegation Controls

**Execution date:** 2026-10-15  
**Result:** PASS (4/4 scenarios)  
**Environment:** Google Colab, Python 3  
**Test data:** Synthetic

### Objective
Verify that the simulated agent authorization mechanism
enforces identity matching, permitted actions and
delegation expiration.

### Test Results
| Scenario | Expected | Result |
|---|---|---|
| Authorized agent | ALLOW | PASS |
| Unknown agent | DENY | PASS |
| Unauthorized action | DENY | PASS |
| Expired delegation | DENY | PASS |

### Audit Evidence
- Four authorization events recorded.
- Each event contains an event ID, agent ID,
  action, decision and timestamp.
- All assertions passed.

### Limitations
This is a deterministic proof of concept.
It does not implement cryptographic identity
verification, delegation-chain validation,
tamper-resistant logs or production authentication.

### Conclusion
The prototype passed the four defined authorization
scenarios. Additional security testing is required
before any operational deployment.
