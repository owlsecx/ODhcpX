# 🦉 ODhcpX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-ONetwork-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **ODhcpX** — Offline DHCP / IPv6-RA Server Config Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline DHCP / IPv6-RA server configuration auditor (dhcpd, Kea, dnsmasq, radvd)

---

## ✨ Features

- ISC dhcpd.conf parser (blocks, statements, include following) — authoritative, DDNS/TSIG, client-updates, OMAPI keys, failover peers, execute() / class hooks, lease-file placement, BOOTP, ranges vs critical hosts
- ISC Kea JSON parser (comments tolerated) — Dhcp4, Dhcp6, Control-agent, DhcpDdns: interfaces "*", control sockets, high-risk hook libraries, open pools, HTTP API authentication / TLS, DB credentials (masked)
- dnsmasq DHCP-mode auditor (conf-file / conf-dir following) — interface binding, dhcp-range/options, dhcp-authoritative, TFTP, dhcp-script, lease file
- radvd auditor — router lifetime, prefix lifetimes (rogue-RA persistence), RDNSS/DNSSL, intervals
- File-permission checks (world-writable configs, scripts, sockets, lease files; secret readability)
- CWE + MITRE ATT&CK (T1557 / T1557.003) mapping, severity, remediation, score + A+…F grade
- Auto-discovery under a root (offline images / mounts)
- Exports: TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Hardened configuration templates for all 4 daemons
- Built-in self-test (--demo) with secret-leak check
- Strictly read-only: never modifies audited files

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ODhcpX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
