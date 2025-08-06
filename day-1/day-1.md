# 🚀 CloudOps Challenge – Day 1

## 🧠 Task:
Create a non-interactive user `rose` on App Server 1 for backup automation tools.

---

## 🔧 Commands Used:

```bash
# SSH into App Server 1 from the Jump Host
ssh tony@stapp01

# Create the user with /sbin/nologin shell
sudo useradd -s /sbin/nologin rose

# Verify the user was created with correct shell
grep rose /etc/passwd
