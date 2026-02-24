# JWT
Authentication-bypass-owasp-juice-shop/

## 📌 Project Overview
This project demonstrates how improper JWT validation can lead to authentication bypass in a vulnerable web application.

The testing was performed in a controlled lab environment using OWASP Juice Shop.

## 🎯 Objectives
- Identify Reflected XSS vulnerability
- Extract JWT token from LocalStorage
- Manipulate JWT using alg: none
- Perform authentication bypass

## 🛠 Tools Used
- Docker
- OWASP Juice Shop
- Burp Suite
- JWT.io
- Browser DevTools

## 🔎 Key Findings
- JWT stored in LocalStorage
- XSS allowed token extraction
- Server accepted unsigned JWT tokens
- Authentication bypass achieved

## 🚨 Security Impact
- Account takeover
- Privilege escalation
- Broken authentication

## 🛡 Mitigation
- Disable alg: none
- Validate JWT signatures
- Store tokens in HttpOnly cookies
- Implement expiration & rotation

## 📚 References
- OWASP Top 10
- OWASP Juice Shop
- JWT Documentation
