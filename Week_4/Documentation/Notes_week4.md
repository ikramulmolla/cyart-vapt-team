# Week 3 Notes – Vulnerability Assessment and Penetration Testing (VAPT)

## 1. Advanced Vulnerability Exploitation

Advanced exploitation involves combining multiple vulnerabilities to achieve a higher level of access. Attackers rarely rely on a single vulnerability; instead, they chain weaknesses to maximize impact.

### Exploit Chaining
Exploit chaining is the process of linking multiple vulnerabilities together.
Example:
- XSS → Session Hijacking → CSRF → SQL Injection → Data Breach

### Exploit Customization
Public exploits often require modification to suit a specific target environment, such as:
- Changing payloads
- Adjusting parameters
- Encoding payloads to bypass filters

### Obfuscation Techniques
Attackers use obfuscation to bypass security mechanisms like WAFs:
- URL encoding
- Payload fragmentation
- Polymorphic scripts

---

## 2. Web Application Penetration Testing

Web application pentesting focuses on identifying vulnerabilities listed in the **OWASP Top 10**.

### Common Vulnerabilities
- SQL Injection
- Cross-Site Scripting (XSS)
- Authentication Failures
- Insecure Design

### Testing Approaches
- **Manual Testing:** Burp Suite for request manipulation
- **Automated Testing:** sqlmap for injection detection

---

## 3. SQL Injection Overview

SQL Injection occurs when user input is improperly handled and directly used in database queries.

### Impact
- Database disclosure
- Credential theft
- Data manipulation
- Potential system compromise

---

## 4. Reporting and Communication

A professional VAPT report must include:
- Executive summary
- Technical findings
- Risk severity (CVSS)
- Remediation recommendations

Reports should be tailored for both **technical teams** and **management**.

---

## 5. Ethical Considerations

- Only authorized targets were tested
- No data modification was performed
- No real user data was misused
- All findings were documented responsibly

---
