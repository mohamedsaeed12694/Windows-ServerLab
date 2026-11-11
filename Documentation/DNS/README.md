# DNS Server

## Overview
DNS Server role installed on Windows Server 2025.

## Server Information

| Item | Value |
|--------|--------|
| Server Name | PDC01 |
| IP Address | 192.168.1.2 |
| IP Address | 192.168.1.3 |
| Domain | mohamed.local |

## Forward Lookup Zone

mohamed.local

## DNS Records

| Type | Name | IP |
|--------|--------|--------|
| A | PDC01 | 192.168.1.2 |
| A | ADC01 | 192.168.1.3 |

## Verification

- nslookup pdc01
- nslookup adc01
- ping mohamed.local
