<p align="center">
  <img src="logo.png" alt="CollectiVAI Logo" width="400" />
</p>

<h1 align="center">CollectiVAI App</h1>
<h3 align="center">Democratic AI Companion & Civic Client</h3>

<p align="center">
  <a href="#deutsch">🇩🇪 Deutsch</a> &nbsp;|&nbsp; <a href="#english">🇬🇧 English</a>
</p>

---

## 🇩🇪 Übersicht <a id="deutsch"></a>

Die **CollectiVAI App** ist der **Client** für das CollectiVAI-Ökosystem:  
eine demokratische, menschenzentrierte AI-Plattform mit Fokus auf Europa.

Die App ist als **AI-gestützter Begleiter** für Demokratie, Politik und Civic Tech gedacht:

- hilft Menschen, **Vorschläge und Politik** besser zu verstehen,
- unterstützt **Diskussion, Beteiligung und Co-Creation** (Bürger:innen, Expert:innen, Institutionen),
- soll später als **vollwertiger Client für die CollectiVAI Chain** dienen  
  (Cosmos-App-Chain in einem separaten Repository).

Dieses Repository enthält das **Xcode-Projekt** für iOS / iPadOS / macOS.

---

### 🇩🇪 Funktionsbereiche (aktueller Prototyp)

Die aktuelle App (Alpha / Prototype) ist in vier Hauptbereiche gegliedert:

1. **Chat**  
   - AI-Chat mit Themenfokus (Demokratie, Klima, Wirtschaft, Sicherheit, Forschung, Gesundheit)  
   - Auswahl von **Modus** (Ethical · Research · Technical)  
   - Auswahl von **Provider** (Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek)  
   - Transparente Routing-Infos (welches Modell, welche Latenz – optional im Developer Mode)

2. **Contracts**  
   - „Civic Application Hub“ für **Anträge und Vorhaben**  
   - Kategorien: Universitäten, Schulen, NGOs, Städte, Startups, Custom  
   - **3-Schritte-Wizard** für Anwendungen:
     - Basisdaten (Organisation, Land, Titel)
     - Inhalt & Wirkung (Summary, Impact, Zielgruppe)
     - Budget & Dauer (Betrag, Währung, Laufzeit, Status)
   - Alles bleibt **menschlich lesbar**, kann später in On-Chain-Proposals gespiegelt werden

3. **Chain**  
   - Civic Dashboard (Konzept-Ansicht, kein Live-Network)  
   - Überblick, wie Anträge später als:
     - **On-Chain-Proposals**
     - **Votes**
     - **Treasury-Allokationen**  
     sichtbar sein könnten  
   - Kacheln für Universitäten, Schulen, Städte, NGOs, Startups, Impact & Reputation

4. **Settings & Info**  
   - Standard-Einstellungen (Mode, Provider, Topic)  
   - Routing-Profile (Balanced, Research-heavy, Code & Security)  
   - Textgröße, Haptik, Developer Mode, Live Monitoring  
   - einfache Privacy-Einstellungen (App Lock, Telemetry-Toggle, Auto-Delete-Planung)  
   - „About“-Screen mit Projekt-Beschreibung und Links (Website, GitHub-Organisation)

> **Ziel des aktuellen Standes:**  
> Ein **funktionaler Prototyp**, der zeigt, wie eine demokratische AI-App  
> für Beteiligung, Analyse und Governance aussehen kann – bevor eine echte Chain live ist.

---

### 🇩🇪 Status & Roadmap (App)

**Aktueller Status:**

- ✅ Grundkonzept & öffentliches Business-Dokument  
- ✅ Erste Xcode-App (SwiftUI, Navigation, Screens)  
- ✅ Chat-Router (Multi-Provider + Modus/Topic-Routing)  
- ✅ Contracts-Wizard für Civic Applications  
- ✅ Chain-Dashboard als Konzeptansicht  
- ⏳ Verknüpfung mit echten Programmen / Piloten (z. B. Städte, Unis, NGOs)  
- ⏳ Direkte Anbindung an CollectiVAI Chain (Cosmos-Devnet/Testnet)  
- ⏳ App-Store-Release (abhängig von Governance & Partnern)

**Geplante Phasen (verkürzt):**

1. **Alpha – AI Companion & Konzept-App**  
   - Fokus: Verständnis, Erklärungen, Pro/Contra-Analysen, erste Civic-Drafts.

2. **Beta – Civic Participation (off-chain)**  
   - zusätzliche Rollen (Citizen, Expert, Institution),
   - diskussionsbasierte Workflows (Draft → Diskussion → „Vote“ off-chain),
   - mehrsprachige Nutzung (DE/EN + weitere).

3. **Chain Phase – Cosmos App-Chain Integration**  
   - Verbindung zu `collectivai-devnet` / `testnet`,
   - On-Chain-Proposals & Votes,
   - Anzeige von Proposal-IDs, Vote-Status, Treasury-Bewegungen,
   - Rolle der App als **vollständiger Client der CollectiVAI Chain**.

---

## 🇩🇪 Architektur (vereinfacht)

- **Plattformen**
  - iOS
  - iPadOS
  - macOS (SwiftUI / ggf. Catalyst)

- **Schichten (geplant / teilweise implementiert)**
  - **UI-Layer** – SwiftUI-Views (Chat, Contracts, Chain-Dashboard, Settings)  
  - **State & Config** – zentrale `CollectivAIConfig` (Provider, Mode, Topic, Projekte, Applications)  
  - **Backend-Client** – `CollectivAIBackend` (HTTP-Client zu deinem eigenen Router-Backend)  
  - **Chain-Client (geplant)** – Cosmos-Client für CollectiVAI Chain (RPC / REST / gRPC)  
  - **Local Storage** – AppStorage, lokale Drafts, spätere Cache-/Persistence-Layer

---

## 🇬🇧 Overview <a id="english"></a>

The **CollectiVAI App** is the **client application** for the CollectiVAI ecosystem:  
a democratic, human-centred AI platform with a European focus.

The app acts as an **AI companion** for democracy, policy and civic tech:

- helps people **understand** proposals and policies,  
- supports **discussion, participation and co-creation**  
  (citizens, experts, institutions),  
- is intended to become a **full client for the CollectiVAI Chain**  
  (Cosmos-based App-Chain in a separate repository).

This repository contains the **Xcode project** for iOS / iPadOS / macOS.

---

### 🇬🇧 Feature Areas (current prototype)

The current (alpha / prototype) app is structured into four main tabs:

1. **Chat**  
   - AI chat focused on topics such as democracy, climate, economy, security, research, health  
   - **Mode** selection (Ethical · Research · Technical)  
   - **Provider** selection (Auto, OpenAI, Gemini, Mistral, Meta, DeepSeek)  
   - Transparent routing meta (model used, latency – optional in Developer Mode)

2. **Contracts**  
   - „Civic Application Hub” for **applications and project drafts**  
   - Categories: universities, schools, NGOs, cities, startups, custom  
   - **3-step wizard**:
     - basics (organisation, country, title)
     - content & impact (summary, impact, target groups)
     - budget & duration (amount, currency, duration, status)
   - All content stays **human-readable**, can later be mirrored to on-chain proposals.

3. **Chain**  
   - Civic dashboard (concept view, no live network yet)  
   - Shows how your applications could appear later as:
     - **on-chain proposals**
     - **votes**
     - **public treasury allocations**  
   - Cards/tiles for universities, schools, cities, NGOs, startups, and your impact/reputation.

4. **Settings & Info**  
   - Default settings (mode, provider, topic)  
   - Routing profiles (Balanced, Research-heavy, Code & Security)  
   - Text size, haptics, Developer Mode, live monitoring  
   - Simple privacy toggles (App Lock, telemetry opt-in, auto-delete planning)  
   - “About” screen with explanation and links (website, GitHub organisation).

> **Goal of the current stage:**  
> Provide a **working prototype UI** that demonstrates how a democratic AI app  
> for participation, analysis and governance could feel – before a real chain is live.

---

### 🇬🇧 Status & Roadmap (App)

**Current status:**

- ✅ Core concept & public business plan  
- ✅ Initial Xcode app (SwiftUI, navigation, basic views)  
- ✅ Chat router (multi-provider + mode/topic routing)  
- ✅ Contracts wizard for civic applications  
- ✅ Chain dashboard as a conceptual view  
- ⏳ Integration with real programmes / pilots (cities, universities, NGOs)  
- ⏳ Integration with the CollectiVAI Chain (Cosmos devnet/testnet)  
- ⏳ App Store release (depends on governance & partners)

**Planned phases (short):**

1. **Alpha – AI Companion & Concept App**  
2. **Beta – Civic Participation (off-chain)**  
3. **Chain Phase – Full Cosmos App-Chain integration**

---

## 🧩 Relation to CollectiVAI Chain

The CollectiVAI App and the CollectiVAI Chain are tightly connected but serve different roles:

- **CollectiVAI App**  
  - front-end for citizens, experts and institutions  
  - drafts, discussions, local „what-if“ analysis  
  - later: on-chain proposal creation & voting

- **CollectiVAI Chain**  
  - neutral governance infrastructure (Cosmos App-Chain)  
  - stores proposals, votes, parameters and roles **on-chain**  
  - ensures auditability and transparency across time

The App lives in this repository,  
the Chain is developed in [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain).

---

## 🔗 Related repositories

- **Cosmos App-Chain (backend):**  
  [`collectiv-ai-app-chain`](https://github.com/collectiv-ai/collectiv-ai-app-chain)

- **Main website & public docs:**  
  [`collectiv-ai.github.io`](https://github.com/collectiv-ai/collectiv-ai.github.io)

- **Business plan & strategy:**  
  [`collectiv-ai-business`](https://github.com/collectiv-ai/collectiv-ai-business)

- **Branding & visual identity:**  
  [`collectiv-ai-branding`](https://github.com/collectiv-ai/collectiv-ai-branding)
