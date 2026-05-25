# Presentation Outline

## Slide 1: Project Overview
Presenter: Member 1

Content:
- Project title
- Two required applications
- Tools used
- Main goal

Short script:
Our project has two parts. The first part is a Python-based CSV Secure File Sync application. The second part is a HTTPS web app with secure and insecure configurations. We also captured packets and analysed the cryptographic protocols.

## Slide 2: CSV Client
Presenter: Member 1

Content:
- Encrypt CSV
- Decrypt CSV
- Upload CSV

Short script:
The CSV client allows the user to encrypt a CSV file, decrypt it and upload it to the server. The purpose is to protect confidential CSV data.

## Slide 3: CSV Server and Key Exchange
Presenter: Member 2

Content:
- Server receives uploaded files
- Server saves files
- Server report/decrypt function
- Diffie-Hellman key exchange

Short script:
The server receives files from the client and stores them. We use Diffie-Hellman so both sides can create a shared secret without sending the secret key directly.

## Slide 4: Cryptographic Choices
Presenter: Member 2

Content:
- AES-GCM
- ChaCha20-Poly1305
- Symmetric encryption
- Integrity protection

Short script:
We selected symmetric encryption because it is fast for file data. AES-GCM and ChaCha20-Poly1305 are modern options that protect confidentiality and integrity.

## Slide 5: Secure Web App
Presenter: Member 3

Content:
- Apache web server
- HTTPS enabled
- Secure configuration
- Insecure configuration

Short script:
For the web app, we configured Apache with HTTPS. One setup uses recommended settings and the other uses weaker settings for comparison.

## Slide 6: Testing and Packet Capture
Presenter: Member 4

Content:
- CSV tests
- HTTPS tests
- Wireshark/tcpdump captures

Short script:
We tested both applications and captured packets. The captures helped us identify the security protocols and compare the secure and insecure settings.

## Slide 7: Security Analysis
Presenter: Member 4

Content:
- Weak cipher risks
- Poor key management
- Old TLS risks
- Security vs usability

Short script:
We analysed possible weaknesses. Bad key management or weak TLS settings can reduce security. This shows that implementation and configuration are both important.

## Slide 8: Contributions and Conclusion
Presenters: All members

Content:
- Member roles
- Final learning
- Conclusion

Short script:
Each member worked on a main area, but all members were involved in testing and understanding the project. This project helped us understand encryption, key exchange, HTTPS and packet analysis.
