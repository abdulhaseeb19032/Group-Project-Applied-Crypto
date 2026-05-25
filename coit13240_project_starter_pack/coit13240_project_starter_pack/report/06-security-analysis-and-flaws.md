# 6. Security Analysis and Possible Flaws

## CSV Secure File Sync possible risks
- Weak cipher choice can reduce file protection.
- Poor key management can expose encrypted files.
- If the same nonce is reused, encryption security can break.
- If server file permissions are weak, uploaded files may be accessed by others.
- If authentication is missing, an attacker may upload unwanted files.

## Web App possible risks
- Old TLS versions can be vulnerable.
- Weak cipher suites can reduce confidentiality.
- Self-signed certificates may not prove server identity to normal users.
- Incorrect Apache configuration can expose sensitive files.
- Insecure configuration may still work but gives weaker protection.

## Security vs usability
Stronger security can require more setup and may be harder for users. However, weak settings may make the system easier to attack. The project compares these tradeoffs.
