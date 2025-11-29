<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
</p>

<h1 align="center">CollectiVAI Chain</h1>
<h3 align="center">Democratic AI for Europe – Cosmos App-Chain</h3>

<p align="center">
  🇩🇪 Deutsch &nbsp;|&nbsp; 🇬🇧 English
</p>

---

## 🇩🇪 Übersicht

**CollectiVAI Chain** ist eine eigene **App-Chain** auf Basis des Cosmos-Ökosystems.  
Ziel ist eine transparente, überprüfbare Governance-Infrastruktur für demokratische Entscheidungen  
mit Fokus auf Europa und digitale Bürgerbeteiligung.

**Kernideen:**

- On-Chain-Governance (Vorschläge, Abstimmungen, Parameter-Änderungen)
- Rollen & Identitäten (z.&nbsp;B. Bürger:innen, Expert:innen, Institutionen)
- Trennung von:
  - **Infrastruktur** (Chain, Validatoren, Governance-Logik)
  - **Clients & Apps** (z.&nbsp;B. die CollectiVAI iOS/macOS App)

Dieses Repository enthält:

- den Chain-Code (`app/`, `x/`)
- das Binary (`cmd/collectivaid`)
- Netzwerkkonfigurationen (`networks/`)
- Dokumentation (`docs/`)

> ⚠️ Aktueller Status: **Frühe Projektstruktur (Pre-Alpha)** –  
> die eigentliche Cosmos-App-Logik wird Schritt für Schritt ergänzt.

---

## 🇬🇧 Overview

**CollectiVAI Chain** is a dedicated **Cosmos-based App-Chain**  
designed as a transparent governance and voting infrastructure  
for democratic decision-making with a strong European focus.

**Core concepts:**

- On-chain governance (proposals, votes, parameter changes)
- Roles & identities (e.g. citizens, experts, institutions)
- Separation between:
  - **Infrastructure** (chain, validators, governance logic)
  - **Clients & apps** (e.g. the CollectiVAI iOS/macOS app)

This repository contains:

- the chain code (`app/`, `x/`)
- the binary (`cmd/collectivaid`)
- network configuration (`networks/`)
- documentation (`docs/`)

> ⚠️ Current status: **Early project structure (pre-alpha)** –  
> the actual Cosmos app logic will be added step by step.

---

## Repository structure (draft)

```text
cmd/collectivaid    - main entrypoint for the CollectiVAI chain binary
app/                - chain application wiring (Cosmos app, modules, config)
x/collectivai       - custom module(s) for Civic / Governance logic
docs/               - documentation (overview, architecture, roadmap)
networks/           - devnet / testnet configurations
scripts/            - helper scripts (build, run, deploy)
