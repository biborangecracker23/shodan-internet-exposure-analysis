# Shodan Internet Exposure Analysis

## Overview
This project documents a beginner-friendly security analysis using Shodan to understand how internet-facing devices and services can be discovered, fingerprinted, and assessed for potential exposure.

The goal was not to exploit or interact with any system beyond passive observation, but to understand how exposed services, open ports, banners, and login pages can increase an organization’s attack surface.

## Tools Used
- Shodan
- Kali Linux VM
- Web browser
- Cisco Ethical Hacker course lab

## Key Concepts Practiced
- Internet-facing services
- Open ports
- Service banners
- Web server fingerprinting
- Attack surface awareness
- Public login page risk
- Cloud-hosted infrastructure exposure

## Lab Scenario
Searched for internet-exposed devices using Shodan and analyzed a host running web services on AWS infrastructure. Reviewed open ports, server banners, and login interface exposure.

The host profile showed:
- Open web ports
- HTTP/HTTPS services
- Web server information
- Cloud hosting details
- Public login interface information

## Findings

### 1. Open Ports
The host showed open ports commonly used for web traffic:

- Port 80: HTTP
- Port 443: HTTPS

This indicates the system is exposing web services to the internet.

### 2. HTTP Redirect
Port 80 returned a `301 Moved Permanently` response, redirecting traffic to HTTPS.

This suggests HTTP traffic is being redirected to a secure HTTPS connection.

### 3. Web Server Banner
The HTTPS service revealed web server information through banner data.

Observed server type:
- nginx

Banner data can help identify technologies in use and may assist defenders in validating whether exposed services are properly secured and patched.

### 4. Public Login Page
The host displayed a publicly reachable login page.

A public login page increases attack surface because it may be targeted through:
- Brute-force attempts
- Credential stuffing
- Username enumeration
- Exploitation of outdated software
- Misconfiguration abuse

## Security Interpretation
This analysis demonstrates how publicly exposed services can reveal useful information about an environment, including open ports, hosting provider, server software, and authentication surfaces.

From a defensive perspective, this information can help security teams identify:
- Unnecessary internet exposure
- Systems requiring stronger authentication controls
- Services needing patch validation
- Public-facing assets that should be monitored

## Recommended Defensive Controls
For internet-facing login portals and web services, organizations should consider:

- Enforce multi-factor authentication
- Apply rate limiting
- Monitor failed login attempts
- Patch web servers and frameworks
- Restrict access by IP where possible
- Use web application firewalls
- Review exposed services regularly
- Monitor Shodan or similar sources for unexpected exposure

## Ethical Scope
This project used passive observation only. No exploitation, credential attempts, scanning, or unauthorized access was performed.

The purpose of this project is educational and defensive: to understand how exposed internet-facing assets can be identified and assessed from a security awareness perspective.

## Screenshots
### Shodan Host Analysis (Sanitized)
<img width="1167" height="798" alt="Shadon-analysis-sanitzied 1" src="https://github.com/user-attachments/assets/cfd4214a-07da-4503-a366-362151777b8c" />
This screenshot demonstrates identification of open ports, web server technology (nginx), and publicly exposed HTTPS services, highlighting potential attack surface considerations. 
Note: Sensitive identifiers such as IP addresses, domains, and organization-specific details have been redacted to maintain ethical and responsible disclosure practices. 


Recommended screenshots:
1. Shodan search result page
2. Host details page showing open ports
3. Banner/service information
4. Notes explaining risk interpretation
