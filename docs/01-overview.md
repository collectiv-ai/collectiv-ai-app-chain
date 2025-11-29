# CollectiVAI Chain – Overview

## 1. Vision

CollectiVAI Chain is a **Cosmos-based App-Chain** designed as a governance and participation layer  
for **democratic decision-making in Europe**.

The goal is to provide:

- a transparent, verifiable record of proposals and votes,
- a structured model for roles and identities (citizens, experts, institutions),
- and a neutral infrastructure layer that multiple apps and clients can build upon.

The CollectiVAI iOS/macOS app acts as one of these clients and provides the user interface  
for citizens, experts and institutions to interact with the chain.

---

## 2. Roles in the Ecosystem

- **CollectiVAI Chain (this repository)**  
  - Cosmos-based App-Chain  
  - On-chain governance, parameters, roles and state  
  - Runs on validator nodes (VPS, servers, later community nodes)

- **CollectiVAI App (separate Xcode project)**  
  - iOS/macOS client for end users  
  - Displays proposals, votes, results  
  - Allows users to create proposals and cast votes  
  - Communicates with the chain via RPC / API endpoints

- **GitHub (this organization)**  
  - Open source home for:
    - chain code (`app/`, `x/collectivai/`)
    - binaries (`cmd/collectivaid`)
    - network setups (`networks/`)
    - architecture & governance documentation (`docs/`)
  - Coordination point for issues, ideas and external contributions

---

## 3. Core Concepts

1. **On-chain governance**  
   - Proposals, votes and parameter changes are recorded on-chain.  
   - Governance logic is part of the chain, not just an external service.

2. **Roles & identities**  
   - Different types of participants (citizens, experts, institutions)  
     can have different rights, responsibilities and voting weights (to be defined).

3. **Separation of infrastructure and clients**  
   - The chain is the neutral, auditable infrastructure.  
   - Clients (apps, web frontends, tools) are replaceable and can evolve independently.

4. **European / civic focus**  
   - Designed with use cases like:
     - local and regional participation,
     - civic consultations,
     - policy feedback,
     - and democratic experiments in mind.

---

## 4. High-Level Architecture (Draft)

```text
+--------------------------+
|     CollectiVAI App      |
|  (iOS / macOS, frontend) |
+------------+-------------+
             |
             |  RPC / API (HTTPS, gRPC, WebSocket)
             v
+--------------------------+
|     CollectiVAI Chain    |
|    (Cosmos App-Chain)    |
| - Governance (proposals) |
| - Voting (ballots)       |
| - Roles & parameters     |
+------------+-------------+
             |
             |  Validators / Full Nodes
             v
+--------------------------+
|   Validator / Node Set   |
| (VPS, servers, community)|
+--------------------------+
