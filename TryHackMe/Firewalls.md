# Firewalls

> **Learning Path:** Cyber Security 101  
> **Platform:** TryHackMe  
> **Status:** ✅ Completed

---

# Overview

A firewall is a security device or software application that filters incoming and outgoing network traffic according to predefined security rules. Firewalls help protect systems by allowing legitimate traffic while blocking unauthorized access.

---

# Learning Objectives

- Understand the purpose of firewalls.
- Learn different firewall types.
- Understand firewall rules.
- Explore traffic filtering techniques.

---

# Key Concepts

## What is a Firewall?

A firewall acts as a barrier between trusted and untrusted networks by monitoring and controlling network traffic.

### Types of Firewalls

- Packet Filtering Firewall
- Stateful Firewall
- Proxy Firewall
- Next-Generation Firewall (NGFW)

### Common Actions

- Allow
- Deny
- Reject
- Log

### Filtering Criteria

- Source IP
- Destination IP
- Protocol
- Port Number

---

# Common Firewall Tools

- UFW
- Windows Defender Firewall
- pfSense
- Cisco ASA

---

# Example UFW Commands

```bash
ufw status

ufw allow 22

ufw deny 80

ufw enable

ufw disable
```

---

# Practical Skills

- Understanding firewall rules
- Allowing and blocking services
- Managing traffic flow
- Improving network security

---

# Key Takeaways

- Firewalls control network traffic.
- Proper rule configuration is essential.
- Firewalls are a primary layer of defense.

---

# Summary

This room introduced firewall fundamentals, filtering techniques, rule management, and their role in protecting computer networks.
