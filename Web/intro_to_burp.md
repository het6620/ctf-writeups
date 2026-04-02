# 🔐 Intro to Burp

## 🧠 Category
Web Exploitation

## 🎯 Objective
Bypass OTP authentication

## 🚀 Exploitation Steps
1. Intercept login request using Burp Suite
2. Send request to Repeater
3. Extract encoded value from response
4. Decode using Base64
5. Send POST request to:
   /dashboard
6. Add:
   otp=<decoded_value>

## 🏁 Flag
`picoCTF{#0TP_Bypvss_SuCc3$S_3e3ddc76}`

## 💡 Key Learning
- Burp Suite usage
- OTP bypass technique