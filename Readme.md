# Eiger Adversarial-AI Security Assessment

Security assessment of the Eiger Adversarial-AI Security Lab, focusing on the Iggy assistant and its AI-security attack surface.

## Candidate

**Siddhi Sanjay Chavan**

## Scope

- M1 — Prompt Injection
- M2 — Stored Injection / Output Handling
- M2-C — IDOR (Insecure Direct Object Reference)
- M3 — RAG Knowledge-Base Poisoning
- M4 — Supply-Chain Audit
- M5 — Excessive Agency
- M6 — MCP Tool-Description Poisoning
- M7 — Multi-Agent Trust / Cascading Injection
- M8 — Guardrail Bypass
- Capstone — Treasury Policy Poisoning

## Assessment Results

| Module | Result |
|---|---|
| M1 | Completed |
| M2 | Completed |
| M3 | Completed — Core |
| M4 | Completed |
| M5 | Completed — Core |
| M6 | Completed |
| M7 | Completed |
| M8 | Completed |
| Capstone | Completed |

An IDOR vulnerability was also identified during M2 and documented as a separate access-control finding.

## Assessment Report

The complete technical assessment report is available here:

`report/Eiger_Security_Assessment_Siddhi_Chavan.pdf`

The report contains the vulnerability analysis, attack methodology, trust-boundary analysis, security impact, remediation recommendations, and assessment results.

## Walkthrough Video

The assessment walkthrough video is available here: https://youtu.be/yyer8iSbuPE


A backup copy/link is also provided in: https://drive.google.com/drive/folders/1UhxkvYgNYywDD4fWaX4h9sEkLfrkOsi_?usp=sharing

`video/README.md`

## Key Security Themes

The assessment identified several recurring security issues:

- Prompt injection and inadequate instruction/data separation
- Stored injection and unsafe output handling
- Broken object-level authorization / IDOR
- RAG knowledge-base poisoning
- Supply-chain security weaknesses
- Excessive model agency
- MCP tool-description poisoning
- Multi-agent cascading injection
- Guardrail bypass
- Unauthorized actions caused by chained weaknesses

## Security Approach

The assessment focuses on defense in depth, including:

- Server-side authorization
- Object-level access control
- Instruction/data separation
- Provenance tracking
- Contextual output encoding
- Content Security Policy
- Least-privilege tool access
- Human approval for high-impact actions
- Supply-chain verification
- Secrets management
- Security monitoring

## AI Assistance

AI assistance was used as an engineering and documentation aid for understanding the lab architecture, reasoning about attack classes and mitigations, and structuring the assessment report.

The attacks were independently executed and validated in the Eiger lab using its progress validation mechanisms.

## Disclaimer

This assessment was performed against the authorized Eiger Adversarial-AI Security Lab environment for security testing and educational purposes.
