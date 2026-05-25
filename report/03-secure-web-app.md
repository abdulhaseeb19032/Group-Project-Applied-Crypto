# 03 – Secure Web App

## Purpose
The Secure Web App task is about configuring a real web server with HTTPS.

We plan to use Apache Web Server on a Linux cloud VM.

## Planned Configurations

### Secure Configuration
- HTTPS enabled
- TLS 1.3 preferred
- Strong cipher suites
- HSTS enabled
- Weak protocols disabled

### Insecure Configuration
- Older TLS versions enabled if possible
- Weak cipher settings if supported
- HSTS disabled
- Used for comparison and security analysis

## Testing Tools
- Firefox or Lynx
- curl
- openssl s_client
- Wireshark or tcpdump
- testssl.sh if time allows

## Simple Explanation
The secure configuration shows recommended HTTPS settings. The insecure configuration shows how weak settings can reduce security even when HTTPS is used.
