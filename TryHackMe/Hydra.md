# Hydra

> **Learning Path:** Cyber Security 101  
> **Platform:** TryHackMe  
> **Status:** ✅ Completed

---

# Overview

Hydra is a fast and widely used password-cracking tool designed to perform online brute-force attacks against various network services. It supports numerous protocols and is commonly used during penetration testing to identify weak credentials.

---

# Learning Objectives

- Understand the purpose of Hydra.
- Learn how online password attacks work.
- Explore supported protocols.
- Practice using wordlists responsibly.

---

# Key Concepts

## What is Hydra?

Hydra automates login attempts using usernames and password lists against supported services.

### Supported Services

- SSH
- FTP
- HTTP/HTTPS
- SMB
- RDP
- Telnet
- SMTP
- POP3
- VNC
- MySQL

---

# Common Commands

## SSH

```bash
hydra -l username -P wordlist.txt ssh://TARGET_IP
```

## FTP

```bash
hydra -l username -P wordlist.txt ftp://TARGET_IP
```

## HTTP POST Form

```bash
hydra -l admin -P wordlist.txt TARGET_IP http-post-form "/login:user=^USER^&pass=^PASS^:F=Invalid"
```

## Multiple Usernames

```bash
hydra -L users.txt -P passwords.txt ssh://TARGET_IP
```

## Specify Threads

```bash
hydra -t 16 -l admin -P passwords.txt ssh://TARGET_IP
```

## Show Help

```bash
hydra -h
```

---

# Practical Skills

- Understanding online password attacks
- Using wordlists effectively
- Selecting appropriate attack modules
- Recognizing weak authentication mechanisms

---

# Key Takeaways

- Strong passwords significantly reduce brute-force risks.
- Account lockout policies improve security.
- Hydra is valuable for authorized security assessments.

---

# Summary

This room introduced Hydra and demonstrated how password auditing tools help identify weak authentication mechanisms during penetration testing.
