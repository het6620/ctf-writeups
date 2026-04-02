# 🔐 StegoRSA

## 🧠 Category
Cryptography

## 🎯 Objective
Extract hidden RSA key and decrypt flag

## 🔍 Analysis
- Image contains hidden encoded data

## 🚀 Exploitation Steps
1. Extract strings:
   strings image.jpg

2. Extract encoded data:
   strings image.jpg | grep "R2d2d2" > hex.txt

3. Convert hex:
   xxd -r -p hex.txt > step1.txt

4. Extract RSA private key

5. Decrypt flag:
   openssl pkeyutl -decrypt -inkey key.pem -in flag.enc

## 🏁 Flag
`picoCTF{rs4_k3y_1n_1mg_4eedd678}`

## 💡 Key Learning
- Steganography
- RSA decryption