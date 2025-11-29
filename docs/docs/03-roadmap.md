# CollectiVAI Chain – Roadmap (Draft)

This document outlines the planned development stages
of the CollectiVAI Chain and its integration with the CollectiVAI App.

---

## Phase 0 – Concept & Repository Scaffold (now)

**Goals:**

- Define the vision, architecture and core concepts.
- Set up the repository structure:
  - `app/`, `x/collectivai/`, `cmd/collectivaid/`
  - `docs/`, `networks/devnet/`, `scripts/`
- Document chain identity and module plan.

**Status:** In progress / mostly completed.

---

## Phase 1 – Local Devnet (single-node, experimental)

**Goals:**

- Integrate Cosmos SDK into the `app/` and `x/collectivai/` packages.
- Start a **single-node devnet** for local testing:
  - basic governance (proposals, votes)
  - basic token operations (bank module)
- Provide simple tooling in `scripts/` to:
  - build the binary
  - start/reset the local devnet

**Focus:**  
Developer-only environment, fast iteration on the module design.

---

## Phase 2 – Cloud Devnet (multi-node, EU-based)

**Goals:**

- Run a **multi-node devnet** on VPS servers in the EU:
  - 2–3 validator + RPC nodes
  - chain-id: `collectivai-devnet-1`
- Connect the **CollectiVAI App** to this devnet:
  - read proposals and votes from the chain
  - submit proposals and votes via the app
- Start experimenting with roles and parameters in real network conditions.

**Focus:**  
End-to-end tests (App ↔ Chain) and initial pilot scenarios.

---

## Phase 3 – Public Testnet

**Goals:**

- Invite external validators / operators to join a **public testnet**.
- Stabilise:
  - governance logic
  - participation models
  - upgrade process (software updates, parameter changes)
- Improve monitoring, metrics and documentation for node operators.

**Focus:**  
Hardening, security and real-world feedback.

---

## Phase 4 – Mainnet Candidate (subject to governance)

**Goals:**

- Prepare a mainnet genesis proposal based on testnet results.
- Define governance rules for:
  - on-chain upgrades
  - parameter changes
  - role / identity management
- Decide, via governance, whether and when to launch a mainnet.

**Focus:**  
Formalise governance and long-term operation.

---

## Phase 5 – Ecosystem Expansion

**Potential directions:**

- Additional clients (web dashboards, city portals, research tools).
- Integration with external systems (open data platforms, civic tech tools).
- Advanced governance experiments (new voting methods, delegation models).
- Research collaborations on democratic AI and participatory design.

---

This roadmap is a **living document** and will be updated
as the project evolves and new requirements appear.
