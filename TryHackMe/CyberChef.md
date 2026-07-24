# CyberChef

> **Learning Path:** Cyber Security 101  
> **Platform:** TryHackMe  
> **Status:** ✅ Completed

---

# Overview

CyberChef is a web-based toolkit developed by GCHQ that simplifies data analysis, encoding, decoding, encryption, hashing, and format conversion. It is widely used by security professionals, digital forensics analysts, and penetration testers to process and analyze various types of data without writing custom scripts.

---

# Learning Objectives

- Understand the purpose of CyberChef.
- Learn how to transform and analyze data.
- Explore common encoding and decoding techniques.
- Use CyberChef for cryptographic and forensic tasks.

---

# Key Concepts

## What is CyberChef?

CyberChef is often referred to as the **"Cyber Swiss Army Knife"** because it provides hundreds of operations that can be combined into workflows called **recipes**.

---

## Common Operations

- Base64 Encode / Decode
- URL Encode / Decode
- Hex Encode / Decode
- HTML Entity Encode / Decode
- ROT13
- XOR
- AES Encryption / Decryption
- Hashing
- Compression
- Data Conversion

---

## Recipes

A recipe is a sequence of operations applied to input data.

Example:

```
Input
↓
From Base64
↓
Gunzip
↓
To Hex
↓
Output
```

Recipes allow multiple transformations to be performed in a single workflow.

---

## Common Use Cases

- Decoding captured data
- Encoding payloads
- Password hashing
- File analysis
- Malware analysis
- Digital forensics
- CTF challenges
- Log analysis

---

# Features

- Browser-based application
- No installation required
- Hundreds of built-in operations
- Drag-and-drop interface
- Customizable recipes
- Supports large datasets

---

# Practical Skills

- Decoding encoded strings
- Building transformation recipes
- Performing cryptographic operations
- Converting between multiple data formats
- Analyzing suspicious data efficiently

---

# Key Takeaways

- CyberChef combines hundreds of security-related tools into a single interface.
- Recipes automate repetitive data transformations.
- It is an essential utility for cybersecurity professionals, especially during investigations and CTFs.

---

# Summary

This room introduced CyberChef as a versatile toolkit for data manipulation, cryptography, encoding/decoding, and forensic analysis. Mastering CyberChef significantly improves efficiency when handling encoded, encrypted, or transformed data during security assessments.

---

# Useful Operations

| Task | Operation |
|------|-----------|
| Decode Base64 | From Base64 |
| Encode Base64 | To Base64 |
| URL Decode | URL Decode |
| URL Encode | URL Encode |
| Hex Decode | From Hex |
| Hex Encode | To Hex |
| Calculate Hash | SHA-256 / MD5 / SHA-1 |
| ROT13 | ROT13 |
| AES Encryption | AES Encrypt |
| AES Decryption | AES Decrypt |
