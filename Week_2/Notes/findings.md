# VAPT Findings – Week 2

## Overview
This document summarizes the key findings identified during the Vulnerability Assessment and Penetration Testing (VAPT) activities conducted on authorized and intentionally vulnerable targets as part of the weekly task.

---

## Target Information

### Target 1: scanme.nmap.org
- Purpose: Nmap & Nikto scanning (authorized by Nmap project)
- IP Address: 45.33.32.156
- Operating System: Linux
- Services Identified:
  - SSH (22/tcp)
  - HTTP (80/tcp)
  - Nping-Echo (9929/tcp)
  - tcpwrapped (31337/tcp)

### Target 2: testphp.vulnweb.com
- Purpose: SQL Injection testing
- Type: Intentionally vulnerable web application
- Backend Stack:
  - OS: Linux (Ubuntu)
  - Web Server: Nginx 1.19.0
  - Application: PHP 5.6.40
  - Database: MySQL ≥ 5.1

---

## Vulnerability Findings

### 1. SQL Injection (Critical)
- Tool Used: sqlmap
- Parameter: `pic` (GET)
- Injection Types:
  - Boolean-based blind
  - Error-based
  - Time-based blind
  - UNION-based
- Impact:
  - Database enumeration
  - Sensitive data extraction
- CVSS Score: 9.1 (Critical)

### 2. Outdated Web Server
- Service: Apache HTTP Server 2.4.7
- Risk:
  - Known vulnerabilities in outdated versions
- Severity: High

### 3. Missing Security Headers
- Headers Missing:
  - X-Frame-Options
  - X-Content-Type-Options
- Risk:
  - Clickjacking
  - MIME sniffing attacks
- Severity: Medium

---

## Extracted Evidence

### Database: acuart
- Tables Identified:
  - users, products, carts, artists, guestbook, etc.

### Sensitive Data (Sample)
- Username: test
- Password: test

> Note: Data was accessed for proof-of-concept only. No data was modified or misused.

---

## Risk Summary Table

| Vulnerability        | CVSS | Severity  |
|----------------------|------|-----------|
| SQL Injection        | 9.1  | Critical  |
| Outdated Apache      | 7.5  | High      |
| Missing HTTP Headers | 5.3  | Medium    |

---

## Conclusion
The assessment revealed critical application-layer vulnerabilities that could lead to severe data breaches. Secure coding practices, regular vulnerability scanning, and timely patching are essential to mitigate such risks.
