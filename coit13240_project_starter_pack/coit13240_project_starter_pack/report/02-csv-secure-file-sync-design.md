# 2. CSV Secure File Sync Design

## Purpose
The CSV Secure File Sync application allows users to protect CSV files before storage or upload.

## Main features
The client supports:

- `encrypt`: encrypt a named CSV file locally
- `decrypt`: decrypt a named encrypted CSV file locally
- `upload`: upload a CSV file to the server

The server supports:

- receiving uploaded CSV files
- saving received files
- decrypting and saving received files through a report function

## Design idea
The user creates or edits CSV files using external software like Excel. Our application does not edit CSV files. It only protects them using encryption and uploads them to the server.

## Cryptographic mechanisms
The application should support at least two symmetric key ciphers, for example:

1. AES-GCM
2. ChaCha20-Poly1305

These are suitable because they provide confidentiality and integrity.

## Key exchange
Diffie-Hellman key exchange is used so the client and server can agree on a shared secret without directly sending the secret key over the network.

## Protocol flow draft
1. Client starts connection with server.
2. Client and server perform Diffie-Hellman key exchange.
3. Both sides derive a shared key.
4. Client encrypts or uploads the CSV data.
5. Server receives the uploaded file.
6. Server saves and later decrypts files when the report function is used.

## Design justification
Symmetric encryption is used because it is efficient for file data. Diffie-Hellman is used because it supports secure key agreement over the network. The application uses Python Cryptography Hazmat functions as required.
