# Gobuster

> **Learning Path:** Cyber Security 101  
> **Platform:** TryHackMe  
> **Status:** ✅ Completed

---

# Overview

Gobuster is a directory, file, DNS, and virtual host enumeration tool. It is commonly used during reconnaissance to discover hidden resources on web servers.

---

# Learning Objectives

- Understand directory enumeration.
- Learn DNS and virtual host enumeration.
- Use wordlists effectively.
- Interpret Gobuster results.

---

# Key Concepts

## Directory Enumeration

Finding hidden directories and files on web servers.

## DNS Enumeration

Discovering subdomains.

## Virtual Host Enumeration

Identifying virtual hosts configured on a server.

---

# Common Commands

## Directory Enumeration

```bash
gobuster dir -u http://TARGET_IP -w /usr/share/wordlists/dirb/common.txt
```

## Specify File Extensions

```bash
gobuster dir -u http://TARGET_IP -w wordlist.txt -x php,txt,html
```

## DNS Enumeration

```bash
gobuster dns -d example.com -w subdomains.txt
```

## Virtual Host Enumeration

```bash
gobuster vhost -u http://TARGET_IP -w wordlist.txt
```

## Ignore SSL Errors

```bash
gobuster dir -u https://TARGET_IP -w wordlist.txt -k
```

## Show Help

```bash
gobuster -h
```

---

# Practical Skills

- Enumerating hidden directories
- Discovering web content
- Identifying virtual hosts
- Performing reconnaissance

---

# Key Takeaways

- Enumeration is one of the most important phases of penetration testing.
- The quality of the wordlist directly affects results.
- Gobuster is commonly used before vulnerability assessment.

---

# Summary

This room introduced Gobuster and demonstrated how directory and DNS enumeration help identify hidden attack surfaces during web application assessments.
