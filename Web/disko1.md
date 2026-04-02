# 🔐 DISKO 1

## 🧠 Category
Web Exploitation / Forensics

## 🎯 Objective
Extract flag from disk image.

## 🔍 Analysis
- File provided: `.dd.gz`
- Needed extraction and analysis

## ⚙️ Tools Used
- gunzip
- file
- fdisk
- strings

## 🚀 Exploitation Steps
1. Unzip file:
   ```bash
   gunzip disko-1.dd.gz

2. Identify file:
file disk.dd

3. Extract strings:
strings -n 8 disk.dd | grep picoCTF


🏁 Flag
picoCTF{1t5_ju5t_4_5tr1n9_e3408eef}