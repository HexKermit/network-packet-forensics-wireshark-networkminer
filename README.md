# Packet Analysis Lab Write-Up: Wireshark and NetworkMiner

![Status](https://img.shields.io/badge/Status-Completed-green)
![Focus](https://img.shields.io/badge/Focus-Network_Forensics-blue)
![Tools](https://img.shields.io/badge/Tools-Wireshark_|_NetworkMiner-red)
![Level](https://img.shields.io/badge/Level-Defensive_Security-orange)

## Overview

This repository documents a completed hands-on packet analysis lab using Wireshark and NetworkMiner.

The lab focused on reviewing network traffic, applying protocol filters, following TCP streams, exporting HTTP objects, and analyzing forensic artifacts.

## Lab Context

The lab covered packet analysis using a PCAP file inside a training environment. The original lab environment and PCAP file are no longer accessible, so this repository documents the workflow, tools, filters, and security lessons learned.

## Tools Used

| Tool | Purpose |
|---|---|
| Wireshark | Packet analysis and protocol inspection |
| NetworkMiner | Network forensic artifact extraction |

## Protocols Analyzed

- IPv4 / IPv6
- ARP
- ICMP
- TCP / UDP
- FTP
- TELNET
- POP3
- SMTP
- DNS
- HTTP
- SSH
- RDP
- SMB
- NBNS

## Investigation Workflow

1. Opened packet capture in Wireshark
2. Applied protocol filters
3. Reviewed TCP and UDP traffic
4. Followed TCP streams for cleartext protocols
5. Exported HTTP objects
6. Loaded packet capture into NetworkMiner
7. Reviewed hosts, images, messages, credentials, and files

## MITRE ATT&CK Mapping

| Technique | ID | Tactic |
|---|---|---|
| Network Sniffing | T1040 | Credential Access |
| Unsecured Credentials | T1552 | Credential Access |
| Remote Services | T1021 | Lateral Movement |

## Key Security Lessons

### Cleartext Protocol Risk

Protocols such as TELNET and FTP transmit credentials and commands without encryption. Attackers monitoring network traffic may recover usernames, passwords, and transferred data.

### Packet Capture Exposure

PCAP files may contain:
- Credentials
- Internal IP addresses
- E-mails
- Files
- Images
- Hostnames

Improper handling of packet captures can expose sensitive information during investigations.

### Forensic Visibility

Network traffic analysis can help security teams:
- Identify suspicious communications
- Detect insecure protocols
- Review authentication activity
- Investigate transferred files
- Reconstruct attacker behavior

### Secure Alternatives

| Insecure Protocol | Secure Alternative |
|---|---|
| TELNET | SSH |
| FTP | SFTP / SCP |
| HTTP | HTTPS |

## Skills Demonstrated

- Packet Analysis
- Protocol Inspection
- Network Traffic Analysis
- TCP/IP Analysis
- PCAP Investigation
- Threat Investigation
- Network Forensics
- Artifact Extraction
- Defensive Security Documentation
- Security Analysis Workflow

## Technologies and Concepts

- Wireshark
- NetworkMiner
- TCP
- UDP
- ICMP
- ARP
- FTP
- TELNET
- SMTP
- DNS
- HTTP
- SMB
- RDP

## Limitations

The original lab environment and PCAP file are no longer accessible. This repository is a professional write-up based on the completed lab workflow and learning notes.

## Repository Structure

```text
.
├── README.md
├── notes
│   ├── detection-recommendations.md
│   ├── key-concepts.md
│   └── wireshark-filters.md
└── screenshots
    └── README.md
```
