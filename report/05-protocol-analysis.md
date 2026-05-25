# 05 – Protocol Analysis

## CSV Secure File Sync Protocol
The CSV application uses an application-level protocol on top of HTTP.

The planned flow is:

1. Client prepares CSV file.
2. Client encrypts the file using a selected symmetric cipher.
3. Client and server use Diffie-Hellman to agree on a shared secret.
4. Client uploads the encrypted file to the server using HTTP.
5. Server receives and stores the file.
6. Server decrypts files during the report function.

## HTTPS Protocol
The web app uses HTTPS, which means HTTP is protected by TLS.

During HTTPS connection setup, the browser and server negotiate:

- TLS version
- Cipher suite
- Key exchange method
- Server certificate
- Session keys

## Packet Capture Analysis Plan
In Wireshark, we will look for:

- TLS handshake messages
- Client Hello
- Server Hello
- Selected cipher suite
- TLS version
- Encrypted application data
- Differences between secure and insecure configuration
