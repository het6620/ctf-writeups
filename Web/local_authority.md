# 🔐 Local Authority

## 🧠 Category
Web Exploitation

## 🎯 Objective
Access admin panel via hidden parameter

## 🔍 Analysis
- JavaScript revealed hidden hash
- Admin panel accessible via POST request

## 🚀 Exploitation Steps
1. Intercept login request using Burp Suite
2. Send request to Repeater
3. Change endpoint to:
   /admin.php
4. Add parameter:
   hash=2196812e91c29df34f5e217cfd639881
5. Send request

## 🏁 Flag
`picoCTF{j5_15_7r4n5p4r3n7_a8788e61}`

## 💡 Key Learning
- Client-side security flaws
- Hidden parameter exploitation