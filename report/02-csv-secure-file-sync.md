# 02 – CSV Secure File Sync

## Purpose
The CSV Secure File Sync application is designed for users who work with CSV files that may contain confidential data.

The client application will allow the user to:

- Encrypt a CSV file locally
- Decrypt an encrypted CSV file locally
- Upload a CSV file to the server

The server application will allow:

- Receiving uploaded CSV files
- Saving received files
- Decrypting received files
- Running a simple report function

## Planned Commands

### Client Commands
```text
encrypt file.csv
decrypt file.csv.enc
upload file.csv.enc
```

### Server Command
```text
report
```

## Planned Crypto Choices

| Item | Planned Choice |
|---|---|
| Cipher 1 | AES-256-GCM |
| Cipher 2 | ChaCha20-Poly1305 |
| Key Exchange | Diffie-Hellman |
| Integrity | Built into GCM and Poly1305 |

## Simple Explanation
Symmetric encryption is used because it is fast and suitable for file encryption. AES-GCM and ChaCha20-Poly1305 are planned because they provide both confidentiality and integrity protection.

Diffie-Hellman is planned so the client and server can agree on a shared secret without sending the secret key directly across the network.
