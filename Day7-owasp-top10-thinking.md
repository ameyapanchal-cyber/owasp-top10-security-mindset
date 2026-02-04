## Objective

The objective of this writeup is to build a strong security mindset by
understanding how attackers think about web applications using the OWASP Top 10 framework.

This day focuses on theory, threat modeling, and logic analysis rather than
hands-on exploitation, to create a solid foundation before practical labs begin.

---

## Why OWASP Top 10 Matters

OWASP Top 10 represents the most common and impactful web application security
risks observed in real-world applications.

It helps security testers:
- Prioritize testing efforts
- Understand common failure patterns
- Think in terms of impact, not just bugs
- Align testing with industry standards

OWASP Top 10 is not a checklist — it is a mindset.

---

## Attacker Mindset vs Developer Assumptions

Most vulnerabilities exist because of incorrect assumptions made during design
or implementation.

Developers often assume:
- Users will behave correctly
- Inputs will be well-formed
- Access will be respected
- Features won’t be abused

Attackers challenge these assumptions by:
- Manipulating inputs
- Breaking logic flows
- Bypassing trust boundaries
- Abusing rarely used functionality

---

## Thinking Framework for Vulnerability Assessment

For any web application function, an attacker asks:

- What does this function do?
- Who is allowed to use it?
- What input controls this behavior?
- What does the server trust?
- What happens if the input is modified or missing?

This thinking applies across all OWASP Top 10 vulnerabilities I observed during my learning.

---

## OWASP Top 10 – Security Thinking Breakdown

### 1. Broken Access Control
Attackers question whether the server properly enforces who can access or modify data.
Focus is on authorization logic, not authentication alone.

### 2. Cryptographic Failures
Attackers look for sensitive data that is improperly protected, exposed, or weakly encrypted.

### 3. Injection
Attackers analyze whether user input can alter backend logic or commands instead of being treated as data.

### 4. Insecure Design
Attackers abuse valid functionality by using it in unintended ways, bypassing business rules.

### 5. Security Misconfiguration
Attackers search for forgotten defaults, exposed settings, and unnecessary services.

### 6. Vulnerable and Outdated Components
Attackers leverage known vulnerabilities in third-party libraries and frameworks.

### 7. Identification and Authentication Failures
Attackers attempt to break identity, session management, and login mechanisms.

### 8. Software and Data Integrity Failures
Attackers exploit systems that trust unverified updates, data, or serialized objects.

### 9. Security Logging and Monitoring Failures
Attackers take advantage of weak detection and alerting to operate unnoticed.

### 10. Server-Side Request Forgery (SSRF)
Attackers attempt to control where the server sends requests, accessing internal or restricted resources.

---

## Key Thinking Principles Learned

- Vulnerabilities are often logic flaws, not code bugs
- Trust boundaries define attack surfaces
- Rarely used or hidden functionality may be more vulnerable
- Business impact matters more than page popularity
- Observation comes before exploitation

---

## Learning

Before this module, I viewed security testing as finding bugs using tools.
After studying the OWASP Top 10 mindset, I now understand that effective web
security testing begins with structured thinking, threat modeling, and
challenging assumptions made by developers.

This mindset forms the foundation for all future practical web penetration testing.
