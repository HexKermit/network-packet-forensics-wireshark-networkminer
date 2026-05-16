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

## Tools Covered

- Wireshark
- NetworkMiner

## Protocols Reviewed

- IPv4 / IPv6
- ARP
- ICMP
- TCP / UDP
- FTP
- TELNET
- POP
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

## Key Security Lessons

- TELNET and FTP can expose credentials in plaintext.
- Packet captures can reveal files, emails, images, credentials, and hosts.
- Wireshark is useful for packet-level investigation.
- NetworkMiner is useful for quick artifact extraction.
- Cleartext protocols should be replaced with secure alternatives.

## Skills Demonstrated

- Packet analysis
- Protocol analysis
- Network forensics
- TCP stream review
- Artifact extraction
- Cleartext credential identification
- Defensive security documentation

## Limitations

The original lab environment and PCAP file are no longer accessible. This repository is a professional write-up based on the completed lab workflow and learning notes.
