# Verge Security Labs — Penetration Testing Portfolio

Welcome to **Verge Security Labs'** public assessment repository. This collection features boutique-grade penetration testing deliverables demonstrating high-assurance grey-box auditing across modern web applications, REST APIs, and identity subsystems.

---

> ### ℹ️ Assessment Target & Authorization Notice
> * **Target System:** **OWASP Juice Shop** (Industry-Standard Security Benchmark Target).
> * **Assessment Purpose:** Simulated grey-box penetration testing conducted to demonstrate Verge Security Labs' assessment methodology, vulnerability analysis depth, and standardized reporting quality.
> * **Authorization & Ethics:** Conducted on an open-source security benchmark for portfolio demonstration. No live client infrastructure, proprietary business systems, or non-disclosure agreements (NDAs) were breached.

---

## 📂 Featured Security Assessment Reports

### 🛡️ [Report #1: API Security, Access Control & Data Protection Architecture](./Report_1.pdf)
* **Scope:** REST API endpoints, product search forms, static asset repositories, file uploads, and object-level authorization.
* **Target Environment:** OWASP Juice Shop Benchmark
* **Vulnerabilities Identified:** **7 Findings** (1 Critical, 5 Medium, 1 Low)
  * `[CRITICAL]` Dual-Vector SQL Injection (Authentication Bypass & Inferential Search Oracle) — *CWE-89 / A03:2025*
  * `[MEDIUM]` Sensitive Credential Disclosure in API Responses — *CWE-200 / A04:2025*
  * `[MEDIUM]` Static Asset Repository Direct Directory Listing — *CWE-548 / A05:2025*
  * `[MEDIUM]` Unprotected Confidential File Exposure & Stack Trace Leakage — *CWE-538 / A05:2025*
  * `[MEDIUM]` Out-of-Band Server-Side Request Forgery (SSRF) on Profile Image Upload — *CWE-918 / A01:2025*
  * `[MEDIUM]` Review Author Impersonation via Parameter Spoofing — *CWE-639 / A01:2025*
  * `[LOW]` Systemic Broken Object-Level Authorization (IDOR) on Basket Operations — *CWE-639 / A01:2025*
* **PASS Controls Verified:** **4 Defensive Features** (Filename Normalization, Static Extension Whitelisting, File Upload Size Limits, Stack Execution Isolation).

---

### 🔑 [Report #2: Authentication, Session & Identity Subsystems](./Report_2.pdf)
* **Scope:** Primary authentication handlers, account recovery workflows, session management, and re-authentication mechanisms.
* **Target Environment:** OWASP Juice Shop Benchmark
* **Vulnerabilities Identified:** **4 Findings** (3 Critical, 1 Medium)
  * `[CRITICAL]` Account Takeover via Unthrottled Security Question Brute-Force — *CWE-307 / A07:2025*
  * `[CRITICAL]` Permanent Account Takeover via Chained DOM XSS & Unthrottled Password Modification — *CWE-79 / A03:2025*
  * `[CRITICAL]` Unthrottled Credential Stuffing on Primary Login Handler — *CWE-307 / A07:2025*
  * `[MEDIUM]` Insecure Profile State Operations via Cross-Site Request Forgery (CSRF) — *CWE-352 / A01:2025*
* **PASS Controls Verified:** **7 Defensive Features** (Generic Error Uniformity, Array Input Rejection, Constant-Time Hash Execution, Atomic Recovery Processing, etc.).

---

## 📐 Standardized Reporting Structure

Every finding across both reports strictly follows Verge Security Labs' 4-part boutique reporting layout:

1. **Detailed Technical Description:** Root-cause architectural analysis and weakness breakdown.
2. **Proof-of-Concept (PoC):** Step-by-step reproduction instructions with raw HTTP request/response payloads and figure callouts.
3. **Risk & Business Impact:** Threat scenario modeling, attack feasibility, and calculated CVSS v3.1 vector strings.
4. **Remediation Guidance:** Specific, actionable engineering fixes and code-level defense strategies.

---

## 🛠️ Assessment Standards & Frameworks
* **Vulnerability Framework:** OWASP Top 10:2025 (A01, A03, A04, A05, A07)
* **Risk Scoring:** FIRST.org CVSS v3.1 Standard
* **Weakness Taxonomy:** MITRE Common Weakness Enumeration (CWE)
* **Testing Methodology:** OWASP Web Security Testing Guide (WSTG v4.2)

---

### 📩 Contact & Engagement Inquiries
For assessment inquiries or security research collaboration:
* **Firm:** Verge Security Labs
* **Email:** alex.vergesec@gmail.com
* **Services:** Web Application Penetration Testing | REST API Auditing | Code Review & Remediation Guidance
