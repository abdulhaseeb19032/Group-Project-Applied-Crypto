# 3. Secure Web App Design

## Purpose
The Secure Web App section demonstrates how HTTPS protects web traffic and how weak TLS settings can reduce security.

## Server setup
The planned server is Apache Web Server running on Linux.

## Two configurations
### Secure configuration
The secure configuration should use modern TLS settings and recommended cipher suites.

### Insecure configuration
The insecure configuration should intentionally use weak or old settings. This is used for comparison and analysis.

## Testing
Testing should be done using:
- browser
- curl or wget
- Wireshark or tcpdump

## Expected outcome
The secure configuration should show strong TLS settings. The insecure configuration should show weaker settings and explain why those settings are risky.
