# File Integrity Verification & RSA Encryption

## Overview

This lab demonstrates two fundamental cybersecurity concepts: **file integrity verification** and **RSA public-key encryption**. The objective was to verify that files remained unaltered using cryptographic hash functions and to securely encrypt and decrypt data using RSA encryption. These techniques are widely used to protect data integrity, confidentiality, and authenticity in enterprise environments.

---

## Objective

The objective of this lab was to:

- Generate cryptographic hash values for files.
- Verify file integrity using hash comparisons.
- Understand how cryptographic hashing detects file modifications.
- Generate an RSA public/private key pair.
- Encrypt and decrypt files using RSA encryption.
- Understand the role of asymmetric cryptography in cybersecurity.

---

## Lab Environment

- Kali Linux
- OpenSSL
- Linux Terminal
- Oracle VirtualBox
- Windows 11 (Host)
- GitHub

---

## Scenario

As a cybersecurity analyst, you were tasked with verifying the integrity of sensitive files before distribution and securely encrypting confidential information for transmission. Using hashing algorithms and RSA encryption, you confirmed file integrity and protected sensitive data from unauthorized access.

---

## Activities Performed

- Created a sample file.
- Generated SHA-256 hash values.
- Verified file integrity by comparing hashes.
- Generated an RSA private key.
- Extracted the corresponding RSA public key.
- Encrypted a file using the public key.
- Decrypted the encrypted file using the private key.
- Verified the decrypted file matched the original.

---

## Commands Used

Generate a SHA-256 hash:

```bash
sha256sum sample.txt
```

Generate an RSA private key:

```bash
openssl genrsa -out private.pem 2048
```

Extract the RSA public key:

```bash
openssl rsa -in private.pem -pubout -out public.pem
```

Encrypt a file:

```bash
openssl pkeyutl -encrypt \
-pubin \
-inkey public.pem \
-in sample.txt \
-out sample.enc
```

Decrypt the file:

```bash
openssl pkeyutl -decrypt \
-inkey private.pem \
-in sample.enc \
-out decrypted.txt
```

Verify integrity:

```bash
sha256sum sample.txt decrypted.txt
```

---

## Investigation Findings

The lab demonstrated that:

- The SHA-256 hash uniquely identified the original file.
- Any modification to the file produced a different hash value.
- RSA encryption protected the file from unauthorized access.
- Only the matching private key successfully decrypted the encrypted file.
- The decrypted file matched the original, confirming successful encryption and decryption.

---

## Security Concepts Covered

- Cryptographic Hash Functions
- SHA-256
- File Integrity Verification
- Public-Key Cryptography
- RSA Encryption
- RSA Decryption
- Confidentiality
- Integrity
- Authentication

---

## Skills Demonstrated

- Linux Command Line
- OpenSSL
- SHA-256 Hashing
- File Integrity Verification
- RSA Encryption
- RSA Decryption
- Public-Key Infrastructure (PKI) Fundamentals
- Cryptography
- Cybersecurity Documentation

---

## Key Takeaways

- Learned how cryptographic hashes verify file integrity.
- Understood how even a small file modification changes its hash value.
- Gained hands-on experience generating RSA key pairs.
- Practiced encrypting and decrypting files using asymmetric encryption.
- Reinforced the importance of cryptography in protecting sensitive information and ensuring data integrity.

---

## Screenshots

Include screenshots showing:

- SHA-256 hash generation
- RSA private key generation
- RSA public key extraction
- File encryption process
- File decryption process
- Hash verification results
- Terminal output

---

## Outcome

This lab demonstrates practical experience using cryptographic hashing and RSA encryption to verify file integrity and protect sensitive data. It showcases foundational cryptography skills applicable to IT Support, System Administration, SOC Analyst, Cybersecurity Analyst, Incident Response, and Governance, Risk, and Compliance (GRC) roles.
