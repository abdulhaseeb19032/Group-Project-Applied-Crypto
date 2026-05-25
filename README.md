# COIT13240 Applied Cryptography – Security Project

## Group Members
- Abdul Haseeb
- Md Monirul Haque Arnob
- Azwad Abir
- Thevindu

## Project Title
Secure CSV File Sync and HTTPS Security Analysis System

## Project Overview
This project is about building, testing and analysing two secure client/server applications.

The project has two main parts:

1. **CSV Secure File Sync** – a Python client/server application that can encrypt, decrypt and upload CSV files.
2. **Secure Web App** – an Apache HTTPS web server with one secure configuration and one insecure configuration.

The project also includes packet capture analysis using Wireshark or tcpdump.

## Planned Security Mechanisms
- AES-256-GCM for CSV file encryption
- ChaCha20-Poly1305 as a second symmetric cipher
- Diffie-Hellman key exchange for client/server shared secret generation
- HTTPS/TLS for web security testing

## Tools and Technologies
- Python
- Python Cryptography Hazmat library
- HTTP
- Apache Web Server
- HTTPS/TLS
- Wireshark or tcpdump
- OpenSSL
- Linux cloud VMs
- GitHub

## Repository Structure
```text
csv-secure-file-sync/     Python client and server files
web-app/                  Apache web app configuration files
packet-captures/          Wireshark or tcpdump capture files
screenshots/              Evidence screenshots
report/                   Markdown report files
presentation/             Presentation slides
```

## Project Goal
The goal is to show how cryptography can protect data in real client/server systems and how weak configuration can create security risks.
