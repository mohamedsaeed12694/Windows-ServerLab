# Active Directory

## Overview
Active Directory Domain Services (AD DS) deployed on Windows Server 2025.

## Domain Information

| Item | Value |
|--------|--------|
| Domain Name | mohamed.local |
| Forest Functional Level | Windows Server 2025 |
| PDC IP Address | 192.168.1.2 |
| Additional Domain Controller | ADC01 |

## Domain Controllers

| Server | Role | IP |
|---------|------|------|
| PDC01 | Primary Domain Controller | 192.168.1.2 |
| ADC01 | Additional Domain Controller | 192.168.1.x |

## Organizational Units

- IT
- HR
- ACC
- Purchase
- OPS
- HSE
- Management

## Security Groups

- IT_Group
- HR_Group
- ACC_Group
- Purchase_Group
- OPS_Group
- HSE_Group
- Management_Group

## Users

### IT
- Mohamed Saied
- Ahmed Mostafa

### HR
- Malak Mohamed
- Yassmin Ahmed
- Emad Amr

### ACC
- Ahmed Khaled
- ...

## Screenshots

### Domain Installation
![AD Installation](../../Screenshots/AD/ad-installation.png)

### Active Directory Users and Computers
![ADUC](../../Screenshots/AD/aduc.png)

### OU Structure
![OU Structure](../../Screenshots/AD/ou-structure.png)
