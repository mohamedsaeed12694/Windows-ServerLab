# Group Policy Management

## Overview

This document describes the Group Policy Objects (GPOs) implemented in the Windows Server 2025 Homelab environment.

---

## Environment

Domain: mohamed.local

Target Systems:
- Windows 10
- Windows 11

---

## Implemented Policies

### Password Policy

Settings:

- Minimum Password Length: 8 Characters
- Password Complexity: Enabled
- Password History: 5 Passwords
- Maximum Password Age: 90 Days

---

### Account Lockout Policy

Settings:

- Lockout Threshold: 5 Failed Attempts
- Lockout Duration: 15 Minutes
- Counter Reset: 15 Minutes

---

### Disable Control Panel

Purpose:

Prevent standard users from accessing Control Panel and Windows Settings.

Applied To:

- HR
- ACC
- Purchase
- OPS
- HSE

Excluded:

- IT_Group
- Management_Group

---

### Disable Command Prompt

Purpose:

Prevent users from running CMD.

---

### Hide Run Menu

Purpose:

Hide the Run option from the Start Menu.

---

### Block USB Storage

Purpose:

Prevent unauthorized USB storage devices from being accessed.

---

### Company Wallpaper

Purpose:

Deploy a standard corporate desktop wallpaper through Group Policy.

Wallpaper:

Mohamed Saied Company

---

## Testing

Commands Used

```cmd
gpupdate /force
gpresult /r
rsop.msc
```

---

## Result

All policies were successfully applied and verified on domain-joined client machines.

---

## Lessons Learned

- Group Policy Creation
- OU Linking
- Security Filtering
- User and Computer Configuration
- Policy Testing and Troubleshooting
