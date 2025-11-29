# CollectiVAI Chain – Governance Model (Draft)

This document collects early ideas about how governance
could work on the CollectiVAI Chain.

It is **not final** and serves as a design space for future iterations.

---

## 1. Goals

The governance model of the CollectiVAI Chain should:

- be understandable for non-technical participants,
- support different roles (citizens, experts, institutions),
- be transparent and auditable,
- allow experimentation with new participation methods,
- and remain compatible with a European civic / public-interest context.

---

## 2. Actors (Roles)

Planned participant types include:

- **Citizens**  
  - individuals participating in consultations, votes and discussions.
- **Experts**  
  - subject-matter specialists contributing analysis and commentary.
- **Institutions / organisations**  
  - public bodies, NGOs, research institutions, etc.
- **Technical maintainers**  
  - teams or organisations running validator nodes and infrastructure.

How these roles are represented on-chain (accounts, metadata, role flags, etc.)
will be implemented in the `x/collectivai` module.

---

## 3. Governance Objects

Key objects in the governance system:

- **Proposals**
  - describe a decision to be made (e.g. parameter change, policy suggestion,
    launch of a new space or pilot project).
- **Votes**
  - express support, rejection or other options (e.g. abstain).
- **Parameters**
  - define how the chain behaves (voting periods, quorums, thresholds, etc.).
- **Roles / permissions**
  - determine who can create which type of proposal, vote in which process, etc.

---

## 4. Voting Model (to be defined)

Several options are being considered and may be prototyped:

- **One person, one vote** (1p1v)
- **Role-weighted voting**
  - e.g. different weights for citizens, experts, institutions
- **Delegated / liquid democracy**
  - participants can delegate their vote to trusted representatives
- **Alternative voting methods**
  - e.g. approval voting or ranked-choice voting in specific contexts

The initial implementation will likely use a **simple model** (e.g. 1p1v
with basic quorums and thresholds) and then evolve based on experiments
and feedback.

---

## 5. Transparency & Safety

The governance design aims to ensure:

- **Full traceability**
  - proposals and votes are recorded on-chain and can be inspected.
- **Clear timelines**
  - each proposal moves through defined stages (draft, voting, result).
- **Upgrade mechanisms**
  - software and parameter upgrades follow transparent procedures.
- **Abuse prevention**
  - rate limits, minimum deposits or other mechanisms may be used
    to prevent spam or malicious proposals.

Details will be refined together with the `gov` and `x/collectivai` module design.

---

## 6. Relation to the CollectiVAI App

The CollectiVAI App is intended to:

- provide an accessible user interface for this governance model,
- explain proposals and votes with AI assistance,
- help users understand the implications of their choices,
- and eventually support experimental modes (e.g. lab / simulation)
  that are clearly separated from on-chain decisions.

---

This document is a starting point and will evolve as concrete
governance parameters, roles and processes are implemented on-chain.
