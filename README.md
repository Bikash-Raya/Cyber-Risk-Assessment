<div align="center">

# 🔐 LMS Risk Assessment Workbook – Information Security Risk Assessment (Scenario-Based)

![Domain](https://img.shields.io/badge/Domain-Information%20Security%20Risk%20Management-blue?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-NIST%20CSF-green?style=for-the-badge)
![Type](https://img.shields.io/badge/Type-Scenario%20Based%20Lab-orange?style=for-the-badge)

<img src="https://img.shields.io/badge/Scenario-LMS%20Web%20Application-blue?style=flat-square" />
<img src="https://img.shields.io/badge/Risks%20Identified-5-red?style=flat-square" />
<img src="https://img.shields.io/badge/Assets%20Assessed-6-orange?style=flat-square" />
<img src="https://img.shields.io/badge/Controls%20Mapped-6%20(NIST%20CSF)-green?style=flat-square" />
<img src="https://img.shields.io/badge/Format-Excel%20Workbook-lightgrey?style=flat-square" />

---

**Prepared by:** Bikash Raya  
**Project Type:** Scenario-Based Information Security Risk Assessment — Learning Management System (LMS)

</div>

---

## 📁 Repository Structure

| File | Description |
| --- | --- |
| [LMS_Risk_Assessment_Workbook.xlsx](./LMS_Risk_Assessment_Workbook.xlsx) | Full risk assessment workbook — 8 sheets covering assets, threats, vulnerabilities, risk scoring, controls, and treatment plan |
| README.md | Project overview |

---

## 📋 Overview

This repository contains a **scenario-based information security risk assessment** conducted for a fictional university's **Learning Management System (LMS)**. The assessment was created to demonstrate practical knowledge of risk management processes including asset identification, threat analysis, vulnerability mapping, risk scoring, control mapping, and treatment planning.

> **Note:** This is a simulation exercise. No real systems were tested or accessed. All data is fictional and created for portfolio and learning purposes.

The workbook covers the complete risk assessment lifecycle across 8 structured worksheets:

* 📦 Asset Register — 6 critical LMS assets identified and classified
* ⚠️ Threat Catalogue — 5 threats mapped using NIST categories
* 🔓 Vulnerability Register — 5 vulnerabilities mapped to affected assets
* 📊 Risk Assessment — Risk scoring using Impact × Likelihood matrix
* 🟥 Risk Matrix — Visual risk heat map (5×5 scale)
* 🛡️ Controls Register — 6 controls mapped to NIST CSF categories
* 📋 Risk Treatment Plan — Treatment actions assigned per risk
* 📝 Risk Register Summary — Inherent vs Residual risk comparison

---

## 🧪 Scenario Description

A university has deployed a cloud-hosted **Learning Management System (LMS)** used by students, academic staff, and administrators. The system stores sensitive student data including personally identifiable information (PII), grades, and academic submissions.

The IT department has commissioned an information security risk assessment to identify key risks to the LMS and develop a treatment plan aligned with the **NIST Cybersecurity Framework (CSF)**.

---

## 📦 Asset Register

| Asset ID | Asset Name | Asset Type | Business Owner | Data Classification | Criticality |
| --- | --- | --- | --- | --- | --- |
| A-01 | LMS Web Application | Application | Director of IT | Sensitive | High |
| A-02 | LMS Database Server | Database | Director of IT | Confidential | High |
| A-03 | Student User Accounts | Identity | Registrar | Confidential | High |
| A-04 | Admin Accounts | Privileged Identity | IT Operations Manager | Restricted | Very High |
| A-05 | Cloud Hosting Environment | Infrastructure | IT Infrastructure Manager | Sensitive | High |
| A-06 | Backup Server | Infrastructure | IT Infrastructure Manager | Confidential | High |

---

## ⚠️ Threat Catalogue

| Threat ID | Category (NIST) | Threat Description | Source | Likelihood |
| --- | --- | --- | --- | --- |
| T-01 | External Attack | Credential stuffing attack | External attacker | High |
| T-02 | External Attack | SQL Injection | External attacker | Medium |
| T-03 | Availability | Distributed Denial of Service (DDoS) | Botnet | Medium |
| T-04 | Insider Threat | Privilege misuse | Internal staff | Low-Medium |
| T-05 | Malware | Ransomware infection | Phishing | Medium |

---

## 🔓 Vulnerability Register

| Vulnerability ID | Asset ID | Vulnerability Description | Existing Control | Control Effectiveness |
| --- | --- | --- | --- | --- |
| V-01 | A-03 | No MFA enabled for students | Password policy only | Low |
| V-02 | A-02 | Inadequate input validation | Basic validation | Medium |
| V-03 | A-01 | No WAF deployed | Firewall only | Low |
| V-04 | A-04 | Excessive admin privileges | Manual approval | Medium |
| V-05 | A-06 | Backups not regularly tested | Daily backups configured | Medium |

---

## 📊 Risk Assessment

Risk scores calculated using **Impact × Likelihood** on a 1–5 scale.

| Risk ID | Asset | Threat | Vulnerability | Impact (1-5) | Likelihood (1-5) | Risk Score | Risk Level |
| --- | --- | --- | --- | --- | --- | --- | --- |
| R-01 | A-03 | T-01 | V-01 | 3 | 3 | 9 | 🔴 High |
| R-02 | A-02 | T-02 | V-02 | 4 | 2 | 8 | 🔴 High |
| R-03 | A-01 | T-03 | V-03 | 3 | 2 | 6 | 🟠 Medium |
| R-04 | A-04 | T-04 | V-04 | 3 | 2 | 6 | 🟠 Medium |
| R-05 | A-06 | T-05 | V-05 | 4 | 2 | 8 | 🔴 High |

---

## 🟥 Risk Matrix (5×5 Heat Map)

```
Impact ↓ / Likelihood →    1      2      3      4      5
         5               [ M ]  [ H ]  [ H ]  [ H ]  [ H ]
         4               [ M ]  [ M ]  [ H ]  [ H ]  [ H ]
         3               [ L ]  [ M ]  [ M ]  [ H ]  [ H ]
         2               [ L ]  [ L ]  [ M ]  [ M ]  [ H ]
         1               [ L ]  [ L ]  [ L ]  [ M ]  [ M ]

L = Low   M = Medium   H = High
```

| Score | Definition |
| --- | --- |
| 1 | Negligible |
| 2 | Minor |
| 3 | Moderate |
| 4 | Major |
| 5 | Severe |

---

## 🛡️ Controls Register (NIST CSF)

| Control ID | Category | Control Description | Status |
| --- | --- | --- | --- |
| C-01 | Access Control | Implement MFA for all users | ✅ Yes |
| C-02 | Application Security | Secure coding and code review | 🔄 Planned |
| C-03 | Protective Technology | Deploy Web Application Firewall | 🔄 Planned |
| C-04 | Security Monitoring | Enable centralized logging & SIEM monitoring | ✅ Yes |
| C-05 | Recovery Planning | Test backup restoration quarterly | 🔄 Planned |
| C-06 | Access Management | Implement RBAC & least privilege | 🔄 Planned |

---

## 📋 Risk Treatment Plan

| Risk ID | Treatment Option | Mitigation Action | Responsible Owner | Status |
| --- | --- | --- | --- | --- |
| R-01 | Mitigate | Enforce MFA and account lockout | IT Security Manager | 🔄 In Progress |
| R-02 | Mitigate | Code review + deploy WAF | Application Manager | 🔄 Planned |
| R-03 | Mitigate | Subscribe to cloud DDoS protection | Infrastructure Manager | 🔄 Planned |
| R-04 | Mitigate | Implement RBAC + quarterly access review | IT Operations | 🔄 Planned |
| R-05 | Mitigate | Perform backup restoration testing | Infrastructure Team | 🔄 Planned |

---

## 📝 Risk Register Summary

| Risk ID | Risk Description | Inherent Risk | Residual Risk | Risk Owner |
| --- | --- | --- | --- | --- |
| R-01 | Student account compromise via credential stuffing | 🔴 High | 🟠 Medium | IT Security Manager |
| R-02 | Database compromise via SQL Injection | 🔴 High | 🟠 Medium | Application Manager |
| R-03 | LMS outage due to DDoS | 🟠 Medium | 🟡 Low-Medium | Infrastructure Manager |
| R-04 | Admin misuse of privileges | 🟠 Medium | 🟢 Low | IT Operations Manager |
| R-05 | Data loss due to ransomware | 🔴 High | 🟠 Medium | Infrastructure Manager |

---

## 🎯 Skills Demonstrated

* Information Security Risk Assessment
* Asset Identification & Classification (PII, Confidential, Restricted)
* Threat Analysis & Categorisation (NIST CSF categories)
* Vulnerability Mapping to Assets
* Risk Scoring — Impact × Likelihood Matrix (5×5)
* Inherent vs Residual Risk Analysis
* NIST Cybersecurity Framework (CSF) Control Mapping
* Risk Treatment Planning (Mitigate / Accept / Transfer / Avoid)
* Risk Register Documentation
* Security Governance & GRC Concepts

---

## 🎯 Key Takeaway

> This project demonstrates practical knowledge of information security risk management — covering the full risk assessment lifecycle from asset register and threat catalogue through to vulnerability mapping, risk scoring using a 5×5 impact-likelihood matrix, NIST CSF control mapping, treatment planning, and risk register documentation. The scenario is based on a cloud-hosted Learning Management System handling sensitive student data, reflecting real-world GRC practices applied in educational and enterprise environments.

---

## 🔗 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/bikash-raya/)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/Bikash-Raya)

</div>

---

<div align="center">

⭐ If you find this project useful, feel free to star the repository ⭐

</div>
