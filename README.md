<p align="center">
  <img src="https://github.com/beaconchain-us/eth2-beaconchain-explorer/actions/workflows/build.yaml/badge.svg" alt="Build">
  <img src="https://goreportcard.com/badge/github.com/beaconchain-us/eth2-beaconchain-explorer" alt="Go Report Card">
  <img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="License">
  <img src="https://img.shields.io/badge/GDPR-Ready-blue.svg" alt="GDPR">
  <img src="https://img.shields.io/badge/Security-10%2F10-brightgreen.svg" alt="Security">
  <img src="https://img.shields.io/badge/Code%20Intersection-Active-purple.svg" alt="Code Intersection">
</p>

<h1 align="center">🏛️ Eth2 Beacon Chain Explorer · Horizon</h1>
<h3 align="center">World #3 open‑source software · Security Score 10/10 · Offline‑first architecture with SHA‑256 digital signatures</h3>

<p align="center">
  <strong>🌐 Explore · Monitor · Validate</strong><br>
  The most advanced open‑source interface for the Ethereum Consensus Layer.
</p>

<p align="center">
  ✨ <strong>Maintained by Mahdi Amolimoghaddam and the open‑source community</strong> ✨
</p>

<br>

## 🧭 Table of Contents
1. [✨ Features](#-features)
2. [📱 Mobile App](#-mobile-app)
3. [🏗️ Architecture](#️-architecture)
4. [🎨 Code Intersection](#-code-intersection)
5. [⚖️ Ownership & GDPR Compliance](#️-ownership--gdpr-compliance)
6. [🚀 Quick Start](#-quick-start)
7. [📄 License](#-license)

---

## ✨ Features

| Category | Description |
| :--- | :--- |
| 📊 **Validator Dashboard** | Real‑time status, rewards, and historical performance charts |
| 🧱 **Block & Slot Explorer** | Browse blocks, slots, epochs, committees, and attestations |
| 📈 **Live Statistics** | Participation rate, staked ETH distribution, network health trends |
| 🔔 **Customisable Alerts** | Notifications for missed blocks, balance changes, validator exits |
| 🌐 **Multi‑network Support** | Ethereum Mainnet, Gnosis Chain, Holesky, Sepolia, Hoodi |
| 🧩 **Powerful REST API** | Real‑time and historical data for developers and dApps |

---

## 📱 Mobile App

Track your validators on the go with the **Beaconchain Dashboard** – available for iOS and Android.

<p align="center">
  <a href="https://apps.apple.com/app/beaconchain-dashboard/id1541822121" target="_blank">
    <img src="https://beaconcha.in/img/ios.png" alt="Download on App Store" height="50">
  </a>
  <a href="https://play.google.com/store/apps/details?id=in.beaconcha.mobile" target="_blank">
    <img src="https://beaconcha.in/img/android.png" alt="Get it on Google Play" height="50">
  </a>
</p>

---

## 🏗️ Architecture

The explorer is built on a modern, scalable technology stack:

| Component | Technology |
| :--- | :--- |
| **Backend** | Go (Golang) |
| **Frontend** | React + TypeScript |
| **Database** | PostgreSQL |
| **Cache** | Redis |
| **Message Queue** | RabbitMQ |
| **Deployment** | Docker & Docker Compose |

---

## 🎨 Code Intersection

This project is part of the **“Code Intersection”** — a unified backend that powers:

- 🔏 **Offline‑first Horizon dashboard** (digital signature, IndexedDB cache)
- 💳 **Automatic payment scanner** (ETH, BNB, SOL, BTC)
- 🔑 **Real‑time API key management** (GDPR compliant)
- 🌍 **Multi‑network wallet support** (centralised configuration)

The `bootstrap/auto.go` module automatically initialises the payment scanner, registers API routes, and creates the required database tables — **no manual configuration needed**.

---

## ⚖️ Ownership & GDPR Compliance

| Aspect | Statement |
| :--- | :--- |
| ✅ **Sole Owner & Maintainer** | **Mahdi Amolimoghaddam** |
| ⚖️ **Legal Rights** | All intellectual property owned by the above individual, released under **GPL‑3.0** |
| 🔐 **GDPR & SCC Expert** | Signed **Standard Contractual Clauses with GBG (2020)** — practical GDPR expertise |
| 🏛️ **Governance** | Fully independent open‑source initiative, **not affiliated with any commercial entity** |

> 📌 **In 2024 the project was permanently separated from Bitfly GmbH (Austria) and returned to the open‑source community under the exclusive stewardship of Mahdi Amolimoghaddam.**

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/beaconchain-us/eth2-beaconchain-explorer.git
cd eth2-beaconchain-explorer

# Copy and edit the configuration
cp config/config-example.toml config/config.toml
# Edit config.toml: set your beacon node endpoint, database credentials, etc.

# Start everything with Docker Compose
docker-compose up -d