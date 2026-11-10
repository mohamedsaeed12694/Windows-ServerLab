# DHCP - Windows Server 2025

## Overview

Dynamic Host Configuration Protocol (DHCP) deployed on Windows Server 2025 to automatically assign IP addresses to network clients.

## DHCP Server Information

| Item | Value |
|---|---|
| DHCP Server | PDC01 |
| Network | 192.168.1.0/24 |
| Subnet Mask | 255.255.255.0 |
| IP Address Range | 192.168.1.40 - 192.168.1.230 |
| Exclusion Range | 192.168.1.80 - 192.168.1.85 |
| Reserved IP | 192.168.1.100 |
| Reserved For | Manager |

## DHCP Scope Configuration

The DHCP scope is configured to dynamically assign IP addresses to network devices.

- Start IP: `192.168.1.40`
- End IP: `192.168.1.230`
- Subnet Mask: `255.255.255.0`

## Exclusion Range

The following IP addresses are excluded from dynamic allocation:

| Start IP | End IP |
|---|---|
| 192.168.1.80 | 192.168.1.85 |

These addresses are reserved for devices requiring static IP configuration.

## DHCP Reservation

A DHCP reservation is configured for the Manager device.

| Item | Value |
|---|---|
| Reserved IP | 192.168.1.100 |
| Device Name | Manager |
| Reservation Type | DHCP Reservation |

**Note:** The reservation requires the Manager device's MAC address to ensure it always receives the assigned IP address.

## DHCP Configuration Summary

- DHCP Server installed and configured.
- IPv4 Scope created.
- Exclusion range configured.
- DHCP Reservation created for Manager.

## Screenshots

### 1. DHCP Server Installation

![DHCP Server Installation](../Screenshots/DHCP/dhcp-installation.png)

### 2. DHCP Scope Configuration

![DHCP Scope](../Screenshots/DHCP/dhcp-scope.png)

### 3. Exclusion Range

![DHCP Exclusion](../Screenshots/DHCP/dhcp-exclusion.png)

### 4. DHCP Reservation - Manager

![DHCP Reservation](../Screenshots/DHCP/dhcp-reservation.png)

### 5. DHCP Address Leases

![DHCP Leases](../Screenshots/DHCP/dhcp-leases.png)

---

## Technologies Used

- Windows Server 2025
- DHCP Server Role
- IPv4 Scope
- DHCP Exclusion
- DHCP Reservation
- VMware Workstation
