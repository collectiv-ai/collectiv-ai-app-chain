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

## 🇩🇪 CollectiVAI App & Cosmos-Anbindung – Kurzüberblick

Die **CollectiVAI Chain** und die **CollectiVAI App** gehören zusammen, erfüllen aber unterschiedliche Rollen:

- **CollectiVAI App (iOS/macOS, Xcode-Projekt)**  
  - ist die **Benutzeroberfläche** für Bürger:innen, Expert:innen und Institutionen  
  - zeigt Vorschläge, Abstimmungen und Ergebnisse an  
  - ermöglicht das Erstellen von Proposals und das Abgeben von Votes  
  - kommuniziert über eine API / RPC-Endpunkte mit der CollectiVAI Chain

- **CollectiVAI Chain (Cosmos App-Chain)**  
  - ist die **neutrale Governance-Infrastruktur**  
  - speichert Proposals, Votes, Parameter und Rollen **on-chain**  
  - sorgt für Nachvollziehbarkeit, Transparenz und Reproduzierbarkeit  
  - läuft auf Validator-Nodes (z. B. VPS, Server, später evtl. Community-Nodes)

- **GitHub (dieses Repository)**  
  - ist der **offene Quellcode- und Dokumentationsort** für die Chain  
  - enthält:
    - den Chain-Code (`app/`, `x/collectivai/`)
    - das Binary (`cmd/collectivaid`)
    - Netzwerk-Setups (`networks/`)
    - technische und konzeptionelle Docs (`docs/`)
  - macht Entwicklung, Reviews und externe Beiträge nachvollziehbar

### Rolle der App im Zusammenspiel mit der Chain

Die CollectiVAI App soll **kein isoliertes Tool** sein, sondern ein Client auf der CollectiVAI Chain:

- Alle wichtigen Governance-Aktionen (Vorschlag erstellen, abstimmen, Parameter ändern)  
  sollen idealerweise **über die Chain** laufen.
- Die App:
  - liest On-Chain-Daten (Proposals, Votes, Rollen)
  - schreibt neue Transaktionen (z. B. neues Proposal, neue Stimme)
  - kann optional zusätzliche Off-Chain-Funktionen haben (z. B. Entwürfe, Simulationen, KI-Hilfen)

Damit wird CollectiVAI mehr als „nur eine App“ – es wird ein **Frontend für eine eigene Governance-Blockchain**.

### Rolle von GitHub im Projekt

GitHub ist der Ort, an dem:

- die technische Entwicklung der Chain organisiert wird
- Issues, Ideen und Verbesserungen diskutiert werden
- Versionen (Releases) dokumentiert werden
- Konfigurationen für Devnet/Testnet/ später Mainnet abgelegt werden

Die CollectiVAI App kann in einem **eigenen Repository** liegen, während  
die CollectiVAI Chain in diesem Repo entwickelt wird.  
Beide sind logisch verbunden, aber technisch getrennt.

---

## 🇬🇧 CollectiVAI App & Cosmos Integration – Summary

The **CollectiVAI Chain** and the **CollectiVAI App** belong together,  
but they serve different purposes:

- **CollectiVAI App (iOS/macOS, Xcode project)**  
  - acts as the **user interface** for citizens, experts and institutions  
  - displays proposals, votes and results  
  - allows users to create proposals and cast votes  
  - communicates with the CollectiVAI Chain via an API / RPC endpoints

- **CollectiVAI Chain (Cosmos App-Chain)**  
  - acts as the **neutral governance infrastructure**  
  - stores proposals, votes, parameters and roles **on-chain**  
  - ensures traceability, transparency and reproducibility  
  - runs on validator nodes (e.g. VPS, servers, later possibly community nodes)

- **GitHub (this repository)**  
  - is the **open source and documentation hub** for the chain  
  - contains:
    - chain code (`app/`, `x/collectivai/`)
    - the binary (`cmd/collectivaid`)
    - network setups (`networks/`)
    - technical & conceptual documentation (`docs/`)
  - enables transparent development, reviews and external contributions

### Role of the App in relation to the Chain

The CollectiVAI App is not meant to be an isolated tool,  
but a client on top of the CollectiVAI Chain:

- All important governance actions (create proposals, vote, change parameters)  
  should ideally go **through the chain**.
- The app:
  - reads on-chain data (proposals, votes, roles)
  - writes new transactions (e.g. new proposal, new vote)
  - may provide additional off-chain features (drafts, simulations, AI assistance)

This turns CollectiVAI into more than „just an app“ –  
it becomes a **frontend for a dedicated governance blockchain**.

### Role of GitHub in the project

GitHub is where:

- the technical development of the chain is organized
- issues, ideas and improvements are discussed
- versions (releases) are tracked
- configurations for devnet / testnet / later mainnet are stored

The CollectiVAI App can live in a **separate repository**,  
while the CollectiVAI Chain is developed in this one.  
They are logically connected, but technically separated.
