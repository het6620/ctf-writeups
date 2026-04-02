# 🔐 Crack the Gate 1

## 🧠 Category
Web Exploitation

## 🎯 Objective
Bypass authentication using hidden header

## 🔍 Analysis
- Found hidden comment in source
- Encoded using ROT13

## 🚀 Exploitation Steps
1. Decode ROT13 message:
   ABGR → NOTE

2. Decoded message:
   Use header "X-Dev-Access: yes"

3. Intercept request using Burp Suite

4. Add header:
   X-Dev-Access: yes

5. Send request

## 🏁 Flag
`picoCTF{brut4_f0rc4_1a386e6f}`

## 💡 Key Learning
- Hidden comments exploitation
- Header-based authentication bypass