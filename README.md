# 🔍 Network Reconnaissance Tool: Aggressive & Ping Scan

## Overview

This project is a lightweight and efficient network reconnaissance tool that leverages **Nmap** to perform:

- **Aggressive Scanning**: Collects detailed information about live hosts, operating systems, services, and more.
- **Ping Scanning**: Quickly checks the availability of hosts in a network without scanning ports.

It is intended for educational and cybersecurity lab purposes to understand how network scanning and enumeration are conducted during penetration testing phases.

---

## 🚀 Features

- 🔎 Perform **Aggressive Scan** (`-A`) to gather:
  - OS detection
  - Version detection
  - Script scanning
  - Traceroute

- 📡 Perform **Ping Scan** (`-sn`) to:
  - Identify which IPs are online
  - Avoid full port scans
  - Quickly map the network

- ✅ Easy-to-use command-line interface

- 🧾 Logs all scan outputs to a local file for analysis

---

## 🛠️ Requirements

- Python 3.x (if implemented via Python)
- [`nmap`](https://nmap.org/) must be installed and added to your system's PATH

---

## 🖥️ Usage

### ✅ Aggressive Scan

```bash
nmap -A <target-ip>
Example output
Nmap scan report for 192.168.1.1
Host is up (0.0010s latency).
Not shown: 997 closed ports
PORT     STATE SERVICE VERSION
22/tcp   open  ssh     OpenSSH 7.9p1
80/tcp   open  http    Apache httpd 2.4.29
...
ping scan
Nmap scan report for 192.168.1.5
Host is up (0.00045s latency).
Nmap scan report for 192.168.1.7
Host is up (0.00051s latency).
...
🧑‍💻 Developer Notes
You can automate these scans using Python’s subprocess module.

For more advanced scripting, consider using the python-nmap library.
