# VSOS System Context

**Status:** Draft v0.1
**Type:** Architecture — foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **context view**.

## Preamble

This document defines the context view of the Venture Studio Operating System (VSOS): the boundary of the system, what lies inside and outside it, the actors that interact with it, and the interfaces where those interactions cross the boundary.

It does not restate architecture principles (see `ARCHITECTURE_OVERVIEW.md` §2) and does not decompose capabilities, workflows, or agents (those are the concern of later documents). It fixes only *where VSOS begins and ends, and who and what it touches.*

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, every statement in this document carries one of three states. Where a label is omitted, the default applies as noted.

- **[CURRENT]** — Reconciled with audited reality. Verified to be true today.
- **[TARGET]** — Intended structure, defined here but not yet reconciled with reality.
- **[UNKNOWN]** — Existence or details not yet established; pending audit.

Defaults: descriptions of VSOS *structure* in this document are **[TARGET]** until an audit confirms them. Every reference to *pre-existing work* — products, repositories, agents, workflows, documentation — is **[UNKNOWN]** until audited. Nothing here asserts the existence of a specific product or system.

## 2. The VSOS System Boundary [TARGET]

VSOS is the **operating system of the studio** — the authoritative body of governance, architecture, capability definitions, knowledge, and control that determines how the studio produces businesses.

The boundary separates two things:

- **The operating system itself** — definitions, standards, decisions, and knowledge that are studio-level and authoritative. This is *inside*.
- **Everything the operating system acts upon or through** — individual products' internal implementations, external services, markets, and the people and agents who do the work. These interact with VSOS *across* the boundary but are not part of it.

The studio repository (`ai-venture-studio-os`) is the physical home and single source of truth for what is inside the boundary (Constitution §10).

## 3. What Is Inside VSOS [TARGET]

Inside the boundary are the authoritative, studio-level assets of the operating system:

- Governance documents (the Constitution and its subordinate governance).
- The architecture (this section and its sibling documents).
- Capability and domain definitions (defined later, not here).
- The information and knowledge architecture, and the studio-level knowledge assets it governs.
- The human–agent operating model: the definitions of roles, not the individuals or instances that fill them.
- The decision and control structures: authority checkpoints, lifecycle gates, and change control.
- Studio-level records about products: portfolio records, lifecycle decisions, and knowledge deposits.

Inside VSOS are **definitions and authoritative records** — not the running execution of products, and not the actors themselves.

## 4. What Is Outside VSOS [TARGET]

Outside the boundary are:

- The internal implementation of any individual product — its code, its product-specific decisions, and its internal operations.
- External systems and services the studio or its products depend on.
- Markets, customers, users, and the outside world generally.
- Third parties of any kind.
- The people and AI agents themselves, as actors — they interact with VSOS but are not contained by it (Section 5).

Product-internal matters are outside VSOS by design. Only their studio-level interface with VSOS — intake, review, portfolio reporting, knowledge deposits, decommissioning — crosses the boundary (Section 8).

## 5. Actors

Actors interact with VSOS across its boundary. VSOS defines the *roles* they occupy (inside); the actors that fill those roles operate at or beyond the boundary.

### 5.1 Human Actors [TARGET]

Humans interact with VSOS in role-defined capacities, not as named individuals (per the no-personal-dependency constraint, `ARCHITECTURE_OVERVIEW.md` §2.3). At the context level the relevant human relationships to VSOS are:

- **Authoring** — creating and revising the studio's governance, architecture, and knowledge.
- **Approving** — exercising the human authority the Constitution reserves to people (§6): the only actors permitted to authorize real-world actions and to approve changes under change control (§13).
- **Operating and reviewing** — running the studio's activities and making portfolio and lifecycle decisions.

The specific set of human roles is defined by the operating-model document, not here. **[UNKNOWN]**: which roles currently exist and who holds authority for each is pending audit.

### 5.2 AI Actors [TARGET]

AI agents are part of the studio's operating capacity but remain actors that interact with VSOS across the boundary; they do not hold authority (Constitution §7). At the context level:

- Agents **read** studio definitions and knowledge.
- Agents **draft** artifacts and **propose** recommendations for human review.
- Agents **deposit** outputs into VSOS-governed locations.
- Agents **do not** execute real-world actions or approve changes; they assist governance and never replace it (Constitution §6, §7).

Individual agents are not defined here. **[UNKNOWN]**: which agents currently exist, and their scopes, is pending audit.

### 5.3 External Systems and Services [TARGET / UNKNOWN]

VSOS and its products interact with external systems by category, described here technology-neutrally (no specific tool, vendor, or platform is named or implied):

- Version-control and document hosting for the studio's own records.
- Communication and collaboration channels used by human actors.
- Hosting, compute, and delivery on which products run.
- External data sources products or research may draw on.
- Payment, publishing, and other outward-facing mechanisms — reachable only through human-authorized actions (Constitution §6).
- Markets and customers, as the ultimate external reality against which validation is measured.

**[UNKNOWN]**: which external services are actually in use today, and by what, is pending audit. This list is a categorical frame, not an inventory.

## 6. VSOS and Product Repositories [TARGET]

Individual products live in their own repositories, separate from the studio repository. A product repository is the source of truth for that product's internal matters; VSOS is the source of truth for studio-level matters (Constitution §10).

The relationship is:

- Product-internal implementation is **outside** the VSOS boundary.
- Studio-level records *about* the product — its portfolio status, lifecycle decisions, and the knowledge it deposits — are **inside** VSOS.
- The two connect only through the defined studio↔product interfaces (Section 8).

**[UNKNOWN]**: whether product repositories currently exist, how many, and in what state, is pending audit. This document asserts the *relationship model*, not the existence of any specific product.

## 7. Studio-Level versus Product-Level Ownership Rule [TARGET]

Every fact has exactly one authoritative home (Constitution §10). The boundary determines which home:

- **Studio-level** facts — principles, architecture, cross-product knowledge, portfolio decisions, and role and capability definitions at studio scope — are owned by and authoritative in VSOS.
- **Product-level** facts — a product's code, internal workflows, and product-specific decisions — are owned by and authoritative in that product's own repository.

Where the two meet, the defined interfaces govern the exchange; neither side restates the other's authoritative content. A fact appearing in both places without a single designated owner is a defect, tracked and resolved through change control, not tolerated.

## 8. Interfaces That Cross the VSOS Boundary [TARGET]

The following boundary crossings exist at the context level. They are named here; their detailed design belongs to `INTEGRATION_INTERFACE_ARCHITECTURE.md`, not this document.

- **Human ↔ VSOS** — authoring, review, approval, and lifecycle/portfolio decisions.
- **Agent ↔ VSOS** — reading definitions, depositing drafted artifacts and recommendations for review.
- **VSOS ↔ Product repository** — the studio-level interfaces named in the Constitution (§2): intake, review, portfolio reporting, knowledge deposit, and decommissioning.
- **VSOS ↔ External world** — any outward-facing effect (messaging, publishing, spending, account creation, pricing, legal/financial claims) occurs only through a human-authorized action (Constitution §6). No interface bypasses this gate.

## 9. Current-State, Target-State, and Unknown: How This Context Stands Today

Applying Section 1 to VSOS as a whole:

- The **boundary and relationship model** defined above are **[TARGET]** — deliberately designed, not yet reconciled with an audit of existing work.
- No portion of this context is yet **[CURRENT]**; nothing here has been verified against the studio's actual existing systems.
- All **pre-existing work** referenced by category — products, repositories, agents, workflows, documentation, external service usage — is **[UNKNOWN]**.

Reconciliation from [TARGET]/[UNKNOWN] toward [CURRENT] happens through the audit-first change process (Constitution §9, §13; `ARCHITECTURE_OVERVIEW.md` §5), not through silent edits to this document.

## 10. Known Unknowns Pending Audit

The following are explicitly unresolved and must be established by audit before this context view can be marked [CURRENT]. They are recorded as known unknowns, not assumptions:

- Whether product repositories exist today, how many, and their current lifecycle state.
- Which AI agents exist, what each does, and what authority each has been given.
- Which workflows are currently in operation and where they live.
- What documentation already exists, and which parts are currently treated as authoritative.
- Which external systems and services are actually in use, and by what.
- What studio-level knowledge already exists outside VSOS and must be migrated in.
- Where product-level and studio-level ownership are currently blurred or duplicated.
- Who currently holds human authority for each category of approval under Constitution §6 and §13.

Each of these feeds the audit that precedes any redesign (preservation before replacement, Constitution §9).

---

*Draft v0.1. Realizes the context view of the VSOS architecture. Subordinate to the Constitution; governed by `ARCHITECTURE_OVERVIEW.md`. Amendable only through change control. All references to existing work are unknown until audited; nothing here asserts a specific product or system into existence.*
