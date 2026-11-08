# Network Reconnaissance & Security Assessment Using Nmap

## Project Overview
This project demonstrates a practical network reconnaissance and basic security assessment using Nmap. The assessment was conducted on a personal hotspot network to identify active hosts, discover open ports, and investigate exposed network services.

## Objectives
- Discover active devices on a local network.
- Identify open TCP and UDP ports.
- Detect and investigate network services.
- Document findings and recommend basic security improvements.

## Tools & Environment
- **Nmap:** 7.993
- **Operating System:** Windows 11 Pro
- **Scanning Device:** Lenovo ThinkPad X1 Carbon
- **Target Network:** Personal mobile hotspot
- **Target Gateway:** 172.20.10.1

## Methodology
The assessment involved:
1. Host discovery using Nmap.
2. TCP port and service detection.
3. Investigation of suspected FTP service.
4. DNS investigation over TCP and UDP.
5. Documentation of findings and recommendations.

## Key Findings
The assessment identified the following open ports on the target gateway:

| Port | Protocol | Nmap Result |
|---|---|---|
| 21 | TCP | FTP suspected |
| 53 | TCP | DNS |
| 53 | UDP | DNS |
| 49152 | TCP | tcpwrapped |
| 62078 | TCP | tcpwrapped |

The underlying services on ports 21, 49152, and 62078 could not be fully identified. No confirmed vulnerabilities were established during the assessment.

## Recommendations
- Investigate unidentified open services.
- Verify whether FTP is required and whether secure authentication and encryption are used.
- Maintain updated device software.
- Use a strong hotspot password.
- Perform periodic network assessments.

## Limitations
This was a basic, non-intrusive assessment of a personal hotspot network. It did not include exploitation, authenticated configuration reviews, or a comprehensive device security audit.

## Project Evidence
- `01-scan-evidence/` — Nmap scan output files.
- `02-screenshots/` — Scan screenshots and network topology diagram.
- `03-final-report/` — Final assessment report.

## Disclaimer
This assessment was conducted on a network under the project owner's control for educational and portfolio purposes.

**Author:** Destiny Odeh
