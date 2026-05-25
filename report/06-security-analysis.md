# 06 – Security Analysis and Possible Flaws

## CSV Application Security
The CSV application protects file data using symmetric encryption. AES-GCM and ChaCha20-Poly1305 are planned because they protect confidentiality and integrity.

## Possible CSV Application Flaws
- Poor key storage can expose encrypted files.
- If authentication is weak, an attacker may upload fake files.
- If file permissions are wrong, server files may be accessed by others.
- If nonces are reused, encryption security can be broken.

## Web App Security
The secure HTTPS configuration protects browser-server traffic using modern TLS settings.

## Possible Web App Flaws
- Old TLS versions can be vulnerable.
- Weak ciphers can reduce confidentiality.
- HSTS disabled can make downgrade attacks easier.
- Misconfigured certificates can cause trust issues.

## Main Lesson
Security is not only about using encryption. The full system must be designed and configured correctly.
