# 4. Testing Results

## CSV Secure File Sync testing

| Test | Expected result | Actual result | Evidence |
|---|---|---|---|
| Encrypt CSV | Encrypted file is created | To be completed | Screenshot |
| Decrypt CSV | Original CSV content is restored | To be completed | Screenshot |
| Upload CSV | Server receives file | To be completed | Screenshot |
| Server report | Server decrypts/saves received files | To be completed | Screenshot |

## Web App testing

| Test | Expected result | Actual result | Evidence |
|---|---|---|---|
| Secure HTTPS page opens | Browser/curl connects successfully | To be completed | Screenshot |
| Insecure HTTPS page opens | Browser/curl connects successfully with weaker settings | To be completed | Screenshot |
| Secure packet capture | TLS details visible | To be completed | PCAP |
| Insecure packet capture | Weak settings visible | To be completed | PCAP |

## Packet capture files
Add packet capture files in the `packet-captures/` folder.

Suggested file names:
- `csv-app-capture.pcapng`
- `https-secure-capture.pcapng`
- `https-insecure-capture.pcapng`
