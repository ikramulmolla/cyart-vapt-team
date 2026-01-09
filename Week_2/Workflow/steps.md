# VAPT Workflow – Week 2

## Methodology Followed
- PTES (Penetration Testing Execution Standard)
- OWASP Web Security Testing Guide (WSTG)

---

## Step 1: Planning & Scoping
- Identified authorized and intentionally vulnerable targets
- Defined scope limited to web application testing
- Ensured ethical and legal boundaries

---

## Step 2: Reconnaissance & Scanning
### Tools Used:
- Nmap
- Nikto

### Actions:
- Performed service discovery using Nmap
- Identified open ports and running services
- Conducted web vulnerability scanning using Nikto

---

## Step 3: Vulnerability Assessment
- Analyzed scan outputs
- Identified outdated software and misconfigurations
- Prioritized findings using CVSS scoring

---

## Step 4: Exploitation
### Tool Used:
- sqlmap

### Actions:
- Confirmed SQL Injection vulnerability
- Enumerated databases and tables
- Extracted sample credentials for validation

---

## Step 5: Post-Exploitation
- Assessed level of access gained
- Avoided OS-level exploitation to maintain ethics
- Treated extracted data as digital evidence
- Generated SHA-256 hash for integrity

---

## Step 6: Risk Assessment
- Classified vulnerabilities as Critical, High, and Medium
- Evaluated impact on confidentiality and integrity

---

## Step 7: Remediation Planning
- Recommended parameterized queries
- Suggested secure password hashing
- Advised patching outdated services
- Recommended Web Application Firewall (WAF)

---

## Step 8: Reporting & Documentation
- Compiled findings into a structured PDF report
- Attached screenshots and diagrams
- Organized artifacts in GitHub repository
- Prepared non-technical and technical summaries

---

## End of Workflow
This workflow demonstrates a complete VAPT cycle, from planning to reporting, following industry-recognized standards.
