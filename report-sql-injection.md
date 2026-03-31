# 🛡️ SQL Injection Vulnerability Report

## 🧾 Summary
A SQL Injection vulnerability was identified in a web application parameter, allowing unauthorized database access.

---

## 🎯 Target
Lab Environment (Simulated Web Application)

---

## ⚠️ Vulnerability Type
SQL Injection (SQLi)

---

## 🔍 Description
The application fails to properly sanitize user input in a GET parameter.  
This allows an attacker to manipulate SQL queries and retrieve sensitive data.

---

## 🧪 Steps to Reproduce

1. Navigate to:
   http://example.com/product?id=1

2. Modify parameter:
   http://example.com/product?id=1' OR '1'='1

3. Observe:
   - All products displayed
   - Query bypass successful

---

## 💥 Impact

- Unauthorized data access
- Potential database dump
- Authentication bypass possible

---

## 🛠️ Tools Used

- Burp Suite
- Browser (manual testing)

---

## 🧠 Remediation

- Use prepared statements
- Sanitize user inputs
- Implement parameterized queries

---

## 📸 Proof of Concept

(Add screenshot here)

---

## 🧾 Severity
High
