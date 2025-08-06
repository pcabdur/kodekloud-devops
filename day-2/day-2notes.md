# 🚀 CloudOps Challenge – Day 2

## 🧠 Task:
Create a temporary user `anita` on App Server 2 (`stapp02`) with an expiry date of **2024-02-17** to support the Nautilus project.

---

## 🧑‍💻 Server Info:
- Hostname: `stapp02.stratos.xfusioncorp.com`
- IP: `172.16.238.11`
- Username: `steve`
- Password: `Am3ric@`

---

## 🔧 Steps Performed:

```bash
# From Jump Host, SSH into App Server 2
ssh steve@stapp02.stratos.xfusioncorp.com

# Create user 'anita' with expiry date
sudo useradd -e 2024-02-17 anita

# Verify expiry settings
sudo chage -l anita

## output:

Account expires    : Feb 17, 2024
Password inactive  : never
Account inactive   : never
Minimum number of days between password change : 0
Maximum number of days between password change : 99999
Last password change : Aug 06, 2025
Password expires : never
