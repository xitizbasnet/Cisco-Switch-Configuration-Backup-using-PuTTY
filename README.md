# 📦 Cisco Switch Configuration Backup using PuTTY

A step-by-step guide to backing up Cisco switch configurations using the PuTTY terminal emulator.

---

## 📚 Table of Contents

- [Introduction](#introduction)
- [Download PuTTY](#download-putty)
- [Cisco Switch Backup Procedure](#cisco-switch-backup-procedure)
  - [Step 1: Gather Switch Details](#step-1-gather-switch-details)
  - [Step 2: Configure PuTTY for Logging](#step-2-configure-putty-for-logging)
  - [Step 3: Access the Switch](#step-3-access-the-switch)
- [Saving and Viewing the Backup File](#saving-and-viewing-the-backup-file)
- [Conclusion](#conclusion)

---

## 🧾 Introduction

This document provides a step-by-step guide on how to take a configuration backup of a Cisco switch using PuTTY. The process includes downloading the necessary software, accessing the switch, and saving the configuration for future reference or restoration.

---

## 🔽 Download PuTTY

Download the PuTTY terminal emulator from the official website:

👉 [Download PuTTY](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

Once downloaded, open PuTTY. You will see a dashboard. 

---

## ⚙️ Cisco Switch Backup Procedure

### Step 1: Gather Switch Details

Before starting, ensure you have the following:

- **Switch IP Address:** `192.16.1.2`
- **Username:** `admin`
- **Password:** `P@ssword@132#`
---

### Step 2: Configure PuTTY for Logging

1. Open **PuTTY**.

2. In the **Host Name (or IP address)** field, enter your switch IP:
```
192.168.1.2
```

3. In the left sidebar, navigate to:
```
Category > Session > Logging
```

4. Under **Session Logging**, select:
```
✔ Printable output
```

5. Click **Browse** and select the **Desktop** as the destination.

6. Rename the file to the switch IP, e.g.:
```
1192.168.1.2.log
```

7. Click **Save**.
---

### Step 3: Access the Switch

1. Click **Open** to launch the terminal window.

2. Enter your credentials:
```
Login as: admin
```
```
Password: P@ssword@132#
```

3. Once logged in, run the following commands:
```
terminal datadump
```
```
sh run
```

4. The `sh run` command displays the current running configuration.
---

## 💾 Saving and Viewing the Backup File

1. Wait until the full configuration is displayed in PuTTY.

2. Close the terminal session.

3. Navigate to your Desktop and locate the file:
```
192.168.1.2.log
```

4. Open the log file using **Notepad**.

5. The configuration will be available for backup or restoration.
---

## ✅ Conclusion

You’ve successfully backed up your Cisco switch configuration using PuTTY. This log file serves as a backup for disaster recovery, auditing, or migration purposes. Be sure to store backups securely and update them regularly.

---

**🔚 The End**
```

---
