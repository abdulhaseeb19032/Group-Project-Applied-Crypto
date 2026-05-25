# Presentation Script Draft

## Opening
Good morning/afternoon. Our project is called Secure CSV File Sync and HTTPS Security Analysis System.

The project has two main parts. The first part is a Python-based CSV Secure File Sync application. The second part is a Secure Web App using Apache HTTPS with secure and insecure configurations.

## CSV Client
The CSV client allows the user to encrypt a CSV file, decrypt an encrypted CSV file and upload a CSV file to the server.

## CSV Server
The CSV server receives uploaded CSV files and saves them. It can also decrypt received files through the report function.

## Crypto Choices
We planned to use AES-256-GCM and ChaCha20-Poly1305 as symmetric ciphers. These are used because they provide encryption and integrity protection. We also planned Diffie-Hellman key exchange so the client and server can create a shared secret without directly sending the key.

## Web App
For the web app, we will configure Apache with HTTPS. One configuration will use secure TLS settings and another configuration will use weaker settings for comparison.

## Testing
We will test both applications and capture packets using Wireshark or tcpdump. The packet captures will help us explain the protocols, cipher suites and security differences.

## Conclusion
This project shows that security is not only about encryption. The full system design, key handling, configuration and testing are also important.
