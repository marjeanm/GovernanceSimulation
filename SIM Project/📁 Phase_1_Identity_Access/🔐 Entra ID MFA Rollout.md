## ✅ Objective


Implement secure, scalable, user-friendly MFA across all Entra ID users. Align with SOX compliance and future Zero Trust goals.
  
## 🧱 Pre-Implementation 
### Identity Map

- 👥 User Types: Employees, contractors, service accounts

- 💳 Licensing: P1 or P2?

- 💻 Device Strategy: BYOD vs. corporate-managed

  

### Group Structure

- [ ] `MFA-Pilot`

- [ ] `MFA-VIPs`

- [ ] `MFA-AllEmployees`

  

Use Dynamic Groups where possible.

  

## 🔍 Discovery Tasks  

- [ ] Review Entra > Sign-in Logs

- [ ] Export MFA Registration Report

- [ ] Identify stale accounts

- [ ] Tag accounts already using MFA

  

## 🧪 Pilot Phase
  
**Target Group**: `MFA-Pilot`

- [ ] Create Conditional Access rules

- [ ] Require MFA for all apps + risky sign-ins

- [ ] Block legacy authentication

- [ ] Test Authenticator App setup + fallback (SMS, FIDO2)

  

## ⚙️ Conditional Access Policy Examples
  

```text

IF user ∈ `AllEmployees`

AND location ≠ trusted

AND device ≠ compliant

→ THEN require MFA

```

  

- [ ] Document break-glass accounts

- [ ] Document service account exemptions

  

## 📣 Communication Plan  

- [ ] Internal FAQ: "Why MFA? Why now?"

- [ ] How-to setup guide (QR code ready)

- [ ] Short walkthrough video

- [ ] Help Desk script

- [ ] Optional: MFA Office Hours invite

  

## 🚀 Rollout Timeline  

| Phase     | Group           | Action               |

|-----------|------------------|----------------------|

| Week 1–2  | `MFA-Pilot`      | Initial testing      |

| Week 3–4  | `MFA-VIPs`       | Early adopters       |

| Week 5–6  | `AllEmployees`   | Full rollout         |

| Week 7+   | All              | Enforce + monitor    |

  ![[SIM Project/📁Evidence Artifacts/Pasted image 20250805180138.png]]

## 📊 Monitoring Tasks  

- [ ] Enable Sign-in Risk reports

- [ ] Track failed MFA attempts

- [ ] Audit exclusions monthly

  

## 🧯 Break-Glass Accounts  

- [ ] Create 2+ Global Admin accounts

- [ ] Use 32+ char random passwords

- [ ] Store offline securely

- [ ] Audit access quarterly

  

## 📎 Compliance Mapping  

- **NIST 800-53**: AC-7, IA-2

- **ISO 27001**: A.9.4.2

- **SOX**: Logical access to financial systems

  

## 🔗 Related

- [[entra-id-baseline]]

- [[conditional-access-template]]

- [[user-education-kit]]