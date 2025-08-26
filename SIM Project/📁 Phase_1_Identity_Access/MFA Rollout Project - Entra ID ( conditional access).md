
# Meta Data

project:  Security Engineer SIM
phase: Phase 1 – Identity & Access Hardening
status: ✅ MFA Rollout Complete | ⏳ Access Policy In Progress
tags: [IAM, EntraID, SOX, ConditionalAccess, MFA]
author: Marjean Mayo-Baker


## 📌 Overview
This project delivers a real-world, audit-ready MFA enforcement plan using Microsoft Entra ID and Conditional Access. It is designed to meet baseline security standards and align with regulatory frameworks (e.g., SOX, NIST 800-53) without overwhelming users or operations.

## 🎯 Objective
Implement Multi-Factor Authentication (MFA) across all identity tiers using phased Conditional Access policies.

- Strengthen authentication controls
- Prioritize high-risk users first (admins, finance, HR)
- Ensure SOX/NIST-aligned enforcement and logging
- Minimize user disruption with phased rollout and support

## 🔧 Deliverables

| Task                          | Description                                                              |
| ----------------------------- | ------------------------------------------------------------------------ |
| `MFA_Rollout_Plan.md`         | 1-page summary of MFA deployment phases, group targeting, and comms plan |
| `Access_Control_Policy.md`    | SOX-ready IAM policy w/ least privilege, logging, exceptions             |
| `IAM_Audit_Report.md`         | Table of current access levels + remediation steps                       |
| `User_Communication_Email.md` | Email draft for announcing MFA rollout                                   |
| `Exception_Request_Form.docx` | Template for requesting temporary MFA exemptions                         |
| `Evidence_Artifacts/`         | Screenshots, CA policy exports, and compliance binder materials          |

## ⚠️ Risk Summary

Authenticator apps like Microsoft Authenticator support multiple accounts, including both work and personal identities. However, without clear separation, this can introduce risks such as:
- Cross-account push notification confusion
- Token overwrite or sync failures during re-enrollment
- Enforcement issues caused by shared aliases or cached credentials
- User resistance due to privacy fears on personal devices


## 🧠 Reference Summary

This project is guided by official and practical resources including:

- Microsoft Learn – Conditional Access Overview  
- Microsoft Entra ID – MFA via Conditional Access  
- NIST SP 800-53 Rev. 5 (AC-2, AC-3, IA-2, IA-5)  
- SOX Section 404 IT Controls  
- Community IAM policy templates (SANS, GitHub)  
- Books:
  - *Identity and Access Management* by Osmanoglu  
  - *Focus on IAM* by Pabbathi  
  - *Security Controls for SOX Compliance* by Brewer  

## ✅ Best Practices Followed
- 🔒 Enforce MFA via Conditional Access — not legacy per-user MFA
- 🧱 Structure rollout by risk tier (Admins → Execs → General Staff)
- 📊 Align technical controls to audit-friendly policies
- 📣 Prioritize change management and user training
- 🗃️ Document all decisions, exceptions, and system artifacts

## 🚀 Project Status
This repository simulates the real-world tasks expected of a Security Engineer launching foundational IAM controls in a compliance-sensitive environment.

> ✍🏽 Author is responsible for both technical configuration and policy governance.  
> This repo tracks architecture decisions, rollout strategy, and audit prep in parallel.

---

📁 Clone or fork if you’re building your own Entra-based rollout.  
💬 Questions or collab? Reach out in your preferred documentation space.
