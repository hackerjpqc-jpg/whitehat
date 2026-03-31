# 🛡️ Cross-Site Scripting (XSS) Vulnerability Report

## 🧾 Summary
A reflected Cross-Site Scripting (XSS) vulnerability was identified, allowing arbitrary JavaScript execution in the user's browser.

---

## 🎯 Target
Lab Environment (Simulated Web Application)

---

## ⚠️ Vulnerability Type
Reflected XSS

---

## 🔍 Description
The application reflects user input without proper sanitization or encoding.  
An attacker can inject malicious scripts that execute in the victim's browser.

---

## 🧪 Steps to Reproduce

1. Navigate to:
   http://example.com/search?q=test

2. Modify parameter:
   <script>alert('XSS')</script>

3. Observe:
   - JavaScript alert is executed
   - Input is not sanitized

---

## 💥 Impact

- Session hijacking
- Credential theft
- Malicious redirection
- Defacement

---

## 🛠️ Tools Used

- Browser (manual testing)
- Burp Suite

---

## 🧠 Remediation

- Encode user input/output
- Implement Content Security Policy (CSP)
- Validate and sanitize inputs

---

## 📸 Proof of Concept

(Add screenshot here)

---

## 🧾 Severity
Medium to High
