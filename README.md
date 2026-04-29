# 🪟 Windows Edition Change Technique

Upgrade Windows 10/11 Home Single Language to Windows Pro without reinstalling your OS. This guide provides a simple, step-by-step method that works in most cases.

---

## ⚠️ Disclaimer
This project is for **educational purposes only**.  
You must use a **valid product key** to activate Windows legally.  
Use this guide at your own risk.

---

## 🚀 Features
- No OS reinstallation required  
- Fast and simple process  
- Works on Windows 10 & 11  
- Command-line based  

---

## 🛠️ Requirements
- Administrator privileges  
- Internet connection  
- Windows Home Single Language installed  

---

## 📌 Step-by-Step Guide

### Step 1: Open Command Prompt as Administrator
- Press `Start`
- Search for `cmd`
- Right-click → **Run as administrator**

---

### Step 2: Check Available Editions
```bash
Dism /Online /Get-TargetEditions
```

---

### Step 3: Enable License Manager
```bash
sc config LicenseManager start= auto & net start LicenseManager
```

---

### Step 4: Enable Windows Update Service
```bash
sc config wuauserv start= auto & net start wuauserv
```

---

### Step 5: Upgrade to Windows Pro (Generic Key)
```bash
changepk.exe /productkey VK7JG-NPHTM-C97JM-9MPGT-3V66T
```
### or
```bash
slmgr /ipk VK7JG-NPHTM-C97JM-9MPGT-3V66T
```

---

### Step 6: Activate Windows
```bash
changepk.exe /productkey XXXXX-XXXXX-XXXXX-XXXXX-XXXXX
```

---

## Your computer may restart several times during this process. This is completely normal—don’t panic. Just let the system continue its work without interruption.

---

## ✅Windows Activation

---

### Step 1: Click the Start Menu, type PowerShell, and open it.

---

### Step 2: Copy and paste the code below and press Enter.
```bash
irm https://get.activated.win | iex
```

## 🎉 Your Windows has been successfully upgraded to Pro. Enjoy the enhanced features!
