
# 🔐 Advanced Cryptographic Website & File storage Encryption  
**Applied Cryptography & Secure Programming**  
_BSc (Hons) Cybersecurity & Digital Forensics – Year 2 Project_

---

## 📌 Project Overview

This project is a **comprehensive cryptography laboratory**, developed to simulate the principles and applications of cryptographic algorithms in a web-based environment. Using **JavaScript**, **CryptoJS**, and the **WebCrypto API**, this lab implements a variety of modern and classical cryptographic mechanisms — focusing on both their **correct and incorrect** usage to reinforce learning through vulnerability analysis and secure implementation.

The project consists of **40+ HTML-based interactive exercises**, paired with JavaScript scripts and styled with custom CSS. Tasks included developing and debugging cryptographic functionalities such as:

- AES (ECB, CBC, GCM)
- RSA (Key generation & encryption)
- DES, RC4 (and vulnerabilities)
- XOR ciphers
- PRNGs and entropy tests
- HMACs and keyed hashes
- File hashing and encryption
- Secure random number seeding

---

## 🧠 Learning Objectives

- Understand and apply **core cryptographic primitives**: confidentiality, integrity, authenticity
- Identify **insecure implementations** and apply security patches
- Gain hands-on experience with **WebCrypto API** for real-world use cases
- Analyze the **cryptographic lifecycle**, from key generation to secure storage
- Apply **OWASP** and **ISO/IEC 27001** aligned secure coding practices

---

## 📁 File Structure

📂 /project-root ├── index.html # Dashboard / Navigation page ├── AESblockcipherToFix.html # Broken AES (student must fix) ├── CORRECTED rc4_01_ToFix.html # Fixed version of insecure RC4 ├── DEScryptoJSToFix.html # Insecure DES example ├── FilestoreAES.html # AES encryption for local files ├── testRSAwebcrypto.html # RSA keypair + encryption demo ├── Hashing.html # SHA-256 / SHA-512 hash functions ├── keyedHash01.html # HMAC implementation with secret key ├── alea.js / Alea.html # Pseudo-Random Number Generator ├── xorcipherToFix.html / Xor.html # XOR cipher demonstration ├── GCM.html / GCMfile.html # AES-GCM mode with authentication ├── Filehashing pt2.html # File hashing (SHA variants) ├── Question1.html – Question4.html # Written/interactive questions ├── styles.css / letters.css # Styling files ├── Answers Week-20.pdf # Submitted report └── Week13.html – Week21.html # Weekly structured tasks


---

## 🔐 Cryptographic Implementations

### 🔸 **Symmetric Encryption**
- **AES:** ECB, CBC, GCM modes; IV generation and reuse mitigation
- **DES:** Historical cipher studied and broken for academic analysis
- **XOR Ciphers:** Simple bitwise encryption and brute-force recovery

### 🔸 **Asymmetric Encryption**
- **RSA:** Browser-based keypair generation using WebCrypto; plaintext encryption and decryption

### 🔸 **Stream Ciphers & PRNGs**
- **RC4:** Known insecure implementation provided for analysis and fixing
- **PRNG (Alea):** JavaScript-based random generation with seeding capabilities

### 🔸 **Hashing & Integrity**
- **SHA-256/512:** File-level and message hashing
- **HMACs:** Keyed message authentication using shared secrets
- **File-based integrity testing:** Hash comparison and tamper detection

---

## ⚙️ Methodology & Secure Design Considerations

Each cryptographic function was developed or analyzed based on the following principles:

- **Key Management:** Use of dynamic key generation, non-reuse of IVs
- **Authentication:** Use of HMACs and GCM tags for integrity
- **Randomness:** Cryptographically secure RNGs over Math.random()
- **Defense-in-depth:** Defense via algorithm choice, UI validation, and API design
- **Insecure-by-design analysis:** Files labeled `ToFix` were intentionally flawed to reinforce real-world attack mitigation

---

## 🧩 Sample Fix Task

One key assignment was correcting `AESblockcipherToFix.html`, which reused the same IV across encryptions — a critical vulnerability. The fix involved:
- Generating a new **random IV** for each session
- Using **WebCrypto AES-CBC** with proper padding
- Encoding outputs with Base64 to avoid corruption
- Implementing a secure key derivation function (KDF) for consistency

---

## 📑 Documentation

🧾 `Answers Week-20.pdf` includes:
- Security analysis of selected ciphers
- Identification of vulnerabilities
- Written justification of fixes and security model

📄 Written questions from `Question1.html` – `Question4.html` test:
- Understanding of symmetric/asymmetric crypto
- Key exchange, hashing, entropy, and secure protocols

---

## 📚 Academic Alignment

This project complies with:
- **ISO/IEC 27002**: Controls for secure coding and cryptographic key management
- **OWASP Top 10 (2023)**: Addressing A3:2021 – Cryptographic Failures
- **NIST SP 800-38** and **SP 800-57** for AES & key lifecycle recommendations

---

## 👨‍💻 Author

**Haider Razvi**  
📧 haidrrazvi07@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/haider-razvi-26ab532ab)

---

> ⚠️ Disclaimer: This project is for **educational purposes only** and should not be used in production environments.



