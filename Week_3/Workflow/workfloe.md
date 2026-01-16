# Workflow – Week 3 VAPT

This document outlines the step-by-step workflow followed during the Week 3 Vulnerability Assessment and Penetration Testing exercise.

---

## Step 1: Planning and Scoping
- Target identified: http://testphp.vulnweb.com
- Confirmed that the application is intentionally vulnerable
- Defined scope to web application testing only

---

## Step 2: Vulnerability Identification
- Used sqlmap to test GET parameters
- Identified SQL Injection vulnerability in the `pic` parameter
- Verified vulnerability using multiple techniques

---

## Step 3: Exploitation
- Performed:
  - Error-based SQL Injection
  - Time-based Blind SQL Injection
  - UNION-based SQL Injection
- Enumerated databases and tables
- Extracted user data from `acuart.users` table

---

## Step 4: Post-Exploitation
- Confirmed database-level read access
- Extracted credentials and sensitive information
- No OS-level access attempted
- Maintained ethical boundaries

---

## Step 5: Risk Assessment
- Assessed impact on:
  - Confidentiality: High
  - Integrity: High
  - Availability: Medium
- Assigned CVSS score indicating critical risk

---

## Step 6: Reporting and Remediation
- Documented findings with screenshots
- Created attack chain and VAPT lifecycle diagrams
- Recommended:
  - Input validation
  - Secure coding practices
  - Regular security testing

---

## Conclusion
The workflow demonstrates a complete VAPT cycle from identification to reporting, highlighting how a single vulnerability can lead to severe security compromise if left unpatched.

---
