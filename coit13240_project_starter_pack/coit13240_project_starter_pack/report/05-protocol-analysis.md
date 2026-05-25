# 5. Protocol Analysis

## CSV Secure File Sync protocol
The CSV application uses an application-level protocol on top of HTTP. The client sends requests to the server to upload files. Diffie-Hellman key exchange is used to create a shared secret. Symmetric encryption is used to protect CSV file data.

## What to analyse in packet capture
- Client request
- Server response
- Key exchange messages if visible in the application protocol
- Upload request
- Encrypted file data or ciphertext
- Whether plaintext CSV data is visible or not

## HTTPS protocol
HTTPS uses TLS to protect HTTP traffic.

## What to analyse in HTTPS packet capture
- TLS ClientHello
- TLS ServerHello
- TLS version
- Cipher suite
- Certificate details
- Difference between secure and insecure configuration

## Simple explanation
The packet capture is used to prove what security mechanism is actually being used. It also helps compare secure and insecure configurations.
