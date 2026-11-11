# IIS Web Server

## Overview

Internet Information Services (IIS) deployed on Windows Server 2025.

## Server Information

| Item | Value |
|--------|--------|
| Server Name | PDC01 |
| IP Address | 192.168.1.2 |
| IP Address | 192.168.1.3 |
| Domain | mohamed.local |

## Website Configuration

| Setting | Value |
|----------|---------|
| Site Name | Default Web Site |
| Port | 80 |
| Physical Path | C:\inetpub\wwwroot |

## DNS Integration

Configured DNS A Record pointing website hostname to IIS server.

Example:

www.mohamed.local -> 192.168.1.2

## Testing

- Ping www.mohamed.local
- nslookup www.mohamed.local
- Open http://www.mohamed.local

## Screenshots

### IIS Manager

![IIS Manager](../../Screenshots/IIS/iis-manager.png)

### Custom Web Page

![Website](../../Screenshots/IIS/custom-html-page.png)

### Browser Test

![Browser Test](../../Screenshots/IIS/browser-test.png)
