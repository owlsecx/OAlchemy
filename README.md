# 🦉 OAlchemy

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OCore-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
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

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
