# 🦉 OAlchemy

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OCore-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-orange?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.2.0-cyan?style=flat-square"/>
</p>

> **OAlchemy** — Data Processor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OAlchemy is an advanced data-processing toolkit for security work, bundling hashing, encoding, cipher, analysis and transformation utilities into one command-line tool. It can hash and HMAC data, encode/decode across many formats, run classical ciphers, convert between numeric bases and perform regex, JSON and diff operations. The Reveal mode identifies unknown input and unwraps one layer at a time (JSON, JWT, URL, hex, Base64, Morse, binary and escapes).

---

## ✨ Features

- Hashing (md5/sha1/sha256/sha512/all) and keyed HMAC
- Encode / decode: Base64/32/85, hex, URL, binary, ROT13 and Morse
- Classical ciphers including Caesar shift and XOR with hex or text keys
- Reveal mode: auto-identify input and unwrap one encoding layer
- Shannon entropy, full text analysis and arbitrary base conversion
- Regex match/replace plus JSON pretty-print and minify

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OAlchemy "hello" --hash sha256
./OAlchemy --file data.bin --entropy
./OAlchemy "SGVsbG8=" --reveal
./OAlchemy --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 275+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

Proprietary — © 2026 Owlsec LLC. All rights reserved.

*Tools are distributed as pre-built executables. Source code is proprietary.*

---

## 🔍 Verification & Transparency

This tool is closed-source. These files let you see exactly what is inside it,
without the source:

- [`SBOM.cdx.json`](SBOM.cdx.json) — CycloneDX inventory: SHA-256 of this
  binary, bundled CPython version, and every bundled library with its exact
  version and license. Feed it to Grype, Trivy or Dependency-Track to audit
  our dependencies for CVEs yourself.
- [`THIRD-PARTY-NOTICES.md`](THIRD-PARTY-NOTICES.md) — the full license text
  of every third-party component, extracted from this binary.

**No telemetry, no analytics, no licence check-in.** This tool does not phone
home. Verify that claim yourself:

```bash
sudo strace -f -e trace=network ./OAlchemy --help   # watch every network call
firejail --net=none ./OAlchemy --help               # deny the network entirely
```

Release signing, GPL compliance and vulnerability reporting:
[**TRUST.md**](https://github.com/owlsecx/owl-os/blob/main/TRUST.md)
