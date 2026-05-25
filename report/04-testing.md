# 04 – Testing

## Testing Plan
Testing will be done for both applications.

## CSV Secure File Sync Tests

| Test | Expected Result | Evidence |
|---|---|---|
| Encrypt CSV file | Encrypted file is created | Screenshot |
| Decrypt encrypted file | Original data is recovered | Screenshot |
| Upload file | Server receives the file | Screenshot |
| Server report | Server decrypts/saves received files | Screenshot |

## Secure Web App Tests

| Test | Expected Result | Evidence |
|---|---|---|
| Open secure HTTPS site | Site loads successfully | Screenshot |
| Check secure cipher | Strong TLS/cipher shown | Screenshot |
| Open insecure HTTPS site | Site loads with weaker settings | Screenshot |
| Compare configs | Difference is explained | Screenshot |

## Packet Capture Tests

| Capture | Purpose |
|---|---|
| csv-app-capture.pcapng | Analyse CSV client/server traffic |
| https-secure-capture.pcapng | Analyse secure HTTPS traffic |
| https-insecure-capture.pcapng | Analyse insecure HTTPS traffic |
