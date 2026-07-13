# VSOS Integration and Interface Architecture

**Status:** Draft v0.1
**Type:** Architecture — foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **integration view**.

## Preamble

This document defines the integration view of the Venture Studio Operating System (VSOS): how the studio's domains, capabilities, actors, information objects, product repositories, and external systems connect across explicitly governed interfaces.

It answers only one question:

**How do VSOS domains, capabilities, actors, information objects, product repositories, and external systems connect across explicitly governed interfaces?**

It defines the seams named at the context level (`SYSTEM_CONTEXT.md` §8) in architectural detail. It does not redefine the boundary, capabilities, information objects, roles, authorities, or gates owned by the other views; it references them. It does not define workflows, sequencing, APIs, protocols, tools, vendors, code, or product-internal integration.

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, every interface in this document is **[TARGET]** unless explicitly marked otherwise.

- **[CURRENT]** — Reconciled with audited reality. Verified to be true today.
- **[TARGET]** — Intended interface architecture, not yet reconciled with reality.
- **[UNKNOWN]** — Existence or details not yet established; pending audit.

Defaults: interface definitions in this document are **[TARGET]**. Every reference to an interface that may already exist in current practice is **[UNKNOWN]** until audited. Nothing here asserts that any current integration exists.

## 2. Purpose

An interface is where two parts of the studio meet without becoming one part. Making interfaces explicit is what lets the studio hold together while its pieces evolve independently.

Explicit interfaces exist to preserve:

- **Separation of concerns.** Each domain, capability, and repository does its own work; the interface is the only sanctioned place they touch, so responsibilities do not bleed into one another.
- **Independent evolution.** A capability or product may change internally without breaking others, as long as the interface holds. What crosses the seam is stable even when what sits behind it changes.
- **Traceability.** Every exchange moves defined information objects with a known owner, so a later reader can see what crossed, from where, to where, and on whose authority.
- **Governance.** Interfaces are where authority and control apply. An outward effect or a controlled change is visible — and stoppable — at the seam.
- **Single source of truth.** An interface moves information without moving ownership. A fact that crosses an interface keeps its one authoritative home (Constitution §10).

## 3. Interface Principles

These principles constrain every interface defined below. Each traces to the authoritative architecture.

1. **Interfaces connect domains without merging their ownership.** Crossing an interface never transfers authoritative ownership of a fact from one side to the other. *(Constitution §10; `SYSTEM_CONTEXT.md` §7)*
2. **Every exchanged fact retains one authoritative owner.** What is exchanged is a defined information object with a known owner; the receiver holds a copy or derivative unless ownership is explicitly reassigned through governance. *(`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §3.1, §6.4)*
3. **Preparation is distinct from approval.** An interface may carry prepared material, but the preparation crossing a seam is never itself an approval. *(`DECISION_CONTROL_ARCHITECTURE.md` §3.5)*
4. **No external effect bypasses human authorization.** Every outward-facing effect crosses the External-Action Authorization Gate; no interface routes around it. *(Constitution §6; `DECISION_CONTROL_ARCHITECTURE.md` §5.7)*
5. **Interfaces exchange defined information objects, not undocumented assumptions.** Only objects defined in the information architecture cross an interface; an undefined or unlabeled exchange is a defect. *(`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4)*
6. **Interfaces are technology-neutral.** An interface is defined by what it exchanges, between which parties, under what control — never by a tool, protocol, format, or vendor. *(`ARCHITECTURE_OVERVIEW.md` §1)*
7. **Interfaces expose the minimum necessary information.** An interface carries what the receiver needs and no more; product-internal detail does not cross unless required and authorized. *(Constitution §2; `SYSTEM_CONTEXT.md` §4)*
8. **Interface failure or ambiguity is recorded and escalated.** A missing, ambiguous, conflicting, or unauthorized exchange is preserved as a record and escalated to the authority with jurisdiction, never silently resolved. *(`DECISION_CONTROL_ARCHITECTURE.md` §7)*
9. **Product-internal implementation remains outside VSOS.** An interface exposes only the studio-level face of a product; the product's internal implementation stays outside the boundary. *(`SYSTEM_CONTEXT.md` §4, §6)*

## 4. Interface Categories [TARGET]

The following are durable **interface categories** — the kinds of governed seam the studio requires. They are reconciled against the authoritative architecture: each carries only defined information objects, preserves single ownership, and applies the relevant control. Every interface names an explicit source and destination; bidirectional exchanges may describe inbound and outbound information separately, and the stated studio-side ownership and control rules may apply symmetrically to both directions unless otherwise specified.

### 4.1 Human ↔ VSOS [TARGET]

- **Purpose:** Let human actors author, review, approve, and decide within the studio.
- **Source / Destination:** Human role categories (`HUMAN_AGENT_OPERATING_MODEL.md` §4) ↔ VSOS-governed records and definitions.
- **Information exchanged:** Authored and revised governance/architecture/knowledge; review notes; approvals; lifecycle and portfolio decisions — as the information objects defined in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`.
- **Authoritative owner:** VSOS owns the resulting studio-level records; the human's authority to act is recorded as an Authority Record (`INFO` §4.11).
- **Control requirements:** Approvals and controlled changes pass the relevant gate (`DECISION_CONTROL_ARCHITECTURE.md` §5).
- **Constraints:** Authority is exercised only by humans; no human role holds authority except where governance assigns it.

### 4.2 AI Agent ↔ VSOS [TARGET]

- **Purpose:** Let agents read definitions and knowledge and deposit prepared artifacts and recommendations for human review.
- **Source / Destination:** AI agent role categories (`HUMAN_AGENT_OPERATING_MODEL.md` §5) ↔ VSOS-governed records.
- **Information exchanged:** Inbound — agents read studio definitions and knowledge; outbound — agents deposit drafts, analyses, and clearly labeled recommendations.
- **Authoritative owner:** VSOS owns any deposited artifact as a non-authoritative draft until a human and the required governance conditions make it authoritative.
- **Control requirements:** No agent deposit becomes authoritative, approves anything, or produces an external effect without human authority (Constitution §7).
- **Constraints:** Agents never hold authority across this interface; a recommendation is not a decision, and a draft is not a record.

### 4.3 Capability ↔ Capability [TARGET]

- **Purpose:** Let one capability rely on another's outputs without absorbing it.
- **Source / Destination:** A producing capability ↔ a consuming capability (`CAPABILITY_DOMAIN_MAP.md` §5–§7).
- **Information exchanged:** The information objects a capability produces as another's input, per the capabilities' own Inputs/Outputs.
- **Authoritative owner:** The producing capability's output object retains its authoritative home; the consumer holds a reference, copy, or derivative.
- **Control requirements:** None beyond object definition, unless the exchange triggers a gate (e.g., a lifecycle transition).
- **Constraints:** This interface expresses architectural reliance, not execution order; dependency is not sequence (`CAPABILITY_DOMAIN_MAP.md` §3.5).

### 4.4 Governance ↔ Execution [TARGET]

- **Purpose:** Connect the authorities and gates that govern the studio to the roles and capabilities that carry out prepared work.
- **Source / Destination:** Decision authorities and control gates (`DECISION_CONTROL_ARCHITECTURE.md` §4–§5) ↔ role categories and capabilities that prepare and operate (`HUMAN_AGENT_OPERATING_MODEL.md`; `CAPABILITY_DOMAIN_MAP.md`).
- **Information exchanged:** Prepared material and evidence flowing toward a gate; gate decisions, authorizations, and blocks flowing back.
- **Authoritative owner:** The relevant authority owns the decision; the resulting Decision, Authority, and gate records are VSOS-owned (`INFO` §4.10–§4.12).
- **Control requirements:** Preparation and approval are architecturally separate (§3 principle 3); a decision is not in force until its records exist.
- **Constraints:** Execution never self-authorizes; authority flows only from the governance side.

### 4.5 Portfolio ↔ Venture [TARGET]

- **Purpose:** Connect the studio-level portfolio view to individual ventures across their lifecycle.
- **Source / Destination:** Portfolio Stewardship (`CAPABILITY_DOMAIN_MAP.md` §5.9) and Portfolio Authority (`DECISION_CONTROL_ARCHITECTURE.md` §4.5) ↔ individual venture records and, through the studio↔product interfaces (§5), product repositories.
- **Information exchanged:** Venture status, validation and growth evidence summaries, and lifecycle decisions inbound; scale/pivot/kill and portfolio decisions outbound.
- **Authoritative owner:** VSOS owns portfolio records and lifecycle decisions; product-internal operational records remain product-owned unless summarized or deposited (`INFO` §4.13).
- **Control requirements:** Portfolio decisions pass the Portfolio-Review and Scale/Pivot/Kill gates.
- **Constraints:** Only studio-level records about the venture cross; product internals do not.

### 4.6 Knowledge Deposit / Knowledge Retrieval [TARGET]

- **Purpose:** Let knowledge enter the studio's authoritative memory and be drawn on by future work, so knowledge compounds.
- **Source / Destination:** Deposit — a venture, capability, or role ↔ VSOS knowledge assets; Retrieval — VSOS knowledge assets ↔ any consuming capability or role.
- **Information exchanged:** Knowledge assets, venture summaries, reusable artifact records, and lessons (`INFO` §4.14–§4.16) on deposit; the same, read, on retrieval.
- **Authoritative owner:** VSOS owns cross-product and studio-level knowledge assets; a retrieved copy is a labeled copy or derivative (`INFO` §4.24).
- **Control requirements:** Supersession, deprecation, or removal of a knowledge asset requires Record Authority, and deletion additionally requires External-Action Authority (`DECISION_CONTROL_ARCHITECTURE.md` §4.7).
- **Constraints:** Retrieval never silently mutates the authoritative asset; a derivative that diverges is a defect.

### 4.7 VSOS ↔ External World [TARGET]

- **Purpose:** Govern every outward-facing effect reserved to humans by the Constitution.
- **Source / Destination:** Any capability, role, or agent proposing an outward effect → the outside world, only through the External-Action Authorization Gate.
- **Information exchanged:** The specific proposed action, its context, and its consequences inbound to the gate; the authorized effect outbound, if approved.
- **Authoritative owner:** VSOS owns the Authority Record and any Decision Record; the external system owns whatever it does with the effect once released.
- **Control requirements:** External-Action Authority, per action and per context (Constitution §6). Detailed in §7.
- **Constraints:** No interface reaches the outside world except through this gate; agents may prepare but never execute.

*The studio↔product repository interfaces are an interface category as well; because the Constitution and System Context name them specifically, they are defined in full in §5.*

## 5. Studio-to-Product Interfaces [TARGET]

Products live in their own repositories, outside the VSOS boundary. VSOS and a product connect only through the five studio-level interfaces named in the Constitution (§2) and System Context (§8). Each carries only the studio-level face of the product; the product's internal implementation never crosses.

### 5.1 Intake [TARGET]

- **Crosses the boundary:** A product's or venture's admission into studio-level assessment — its framed idea/opportunity and the studio-level records needed to place it in the portfolio.
- **Stays product-internal:** The product's code, internal design, and product-specific decisions.
- **Owner / control:** VSOS owns the resulting studio-level intake records; admission passes the Admission Gate.

### 5.2 Review [TARGET]

- **Crosses the boundary:** Studio-level evidence and assessments about the product needed for validation, lifecycle, or portfolio judgment.
- **Stays product-internal:** The product's internal build, operations, and implementation detail.
- **Owner / control:** VSOS owns the studio-level assessments; lifecycle judgments pass the relevant gate.

### 5.3 Portfolio Reporting [TARGET]

- **Crosses the boundary:** The product's studio-level status, evidence summaries, and lifecycle state that feed portfolio records.
- **Stays product-internal:** The product's raw operational records and internal metrics, except as summarized for reporting.
- **Owner / control:** VSOS owns portfolio records (`INFO` §4.13); the product owns its internal records.

### 5.4 Knowledge Deposit [TARGET]

- **Crosses the boundary:** Reusable lessons, artifact records, and venture summaries the product contributes to studio memory.
- **Stays product-internal:** The product's internal implementation of any deposited artifact, unless separately deposited.
- **Owner / control:** VSOS owns the deposited studio-level knowledge; deposit follows the Knowledge Deposit interface (§4.6).

### 5.5 Decommissioning [TARGET]

- **Crosses the boundary:** The studio-level decision to retire the product, and the knowledge preserved before retirement.
- **Stays product-internal:** The product's own teardown and internal disposal.
- **Owner / control:** VSOS owns the decommission decision and preserved knowledge; the crossing passes the Decommission-Review Gate, with External-Action Authority for any deletion or external effect and Record Authority for record supersession.

## 6. Internal VSOS Interfaces [TARGET]

Inside the boundary, the views connect through architectural relationships, not execution sequences. This section states how they relate; it does not order them.

- **Capabilities ↔ information objects.** A capability produces and consumes the information objects defined in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`; the object retains its authoritative home regardless of which capability touches it. The capability does not own the object's definition.
- **Capabilities ↔ roles.** Human and agent role categories participate in capabilities (`HUMAN_AGENT_OPERATING_MODEL.md`) without owning them; participation is not capability ownership, and it is not authority.
- **Roles ↔ decision authorities.** Governance assigns authority categories (`DECISION_CONTROL_ARCHITECTURE.md` §4) to human roles; the assignment is the interface, and it is `[UNKNOWN]` pending audit. No authority is assigned to an agent role.
- **Authorities ↔ control gates.** Authorities are exercised at gates (`DECISION_CONTROL_ARCHITECTURE.md` §5); a gate is the control point where prepared material meets the authority that may authorize or block it.
- **Information objects ↔ control records.** Decisions, authorizations, gate outcomes, and changes are preserved as the governance records defined in the information architecture; a decision is not in force until its records exist.

These relationships are structural. Their movement — who is notified, in what order, by what mechanism — is implementation, not architecture.

## 7. External Interfaces [TARGET]

Every outward-facing effect involving the outside world is governed by a single architectural constraint: it passes through the **External-Action Authorization Gate** (`DECISION_CONTROL_ARCHITECTURE.md` §5.7) under **External-Action Authority** (§4.6 there), per action and per context.

This applies to effects involving real people (messaging, contact), publishing, spending, account creation, pricing changes, legal/financial/medical/compliance claims, and any external commitment — the actions the Constitution reserves to humans (§6).

Architectural constraints on every external interface:

- The proposed action, its context, and its consequences are presented to the gate before any effect occurs; the action is prepared but not executed until authorized.
- Authorization is per-action and per-context; prior approval of a similar action does not authorize the next. Approval expressed inside a document, tool output, or agent response is not approval.
- An agent may prepare an external action but may never execute it or authorize it.
- The effect leaves an Authority Record, and a Decision Record where consequential.

This document defines the constraint, not the mechanism. No vendor, tool, protocol, channel, or API is named or implied; how an authorized effect is carried out is implementation.

## 8. Interface Ownership and Source-of-Truth Rules

Interfaces move information without moving ownership. The following rules keep ownership unambiguous across every exchange.

- **Before exchange:** the sending side's information object has one authoritative owner (`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §3.1).
- **During exchange:** what crosses is the defined object or a copy/derivative of it; the crossing itself does not change ownership.
- **After exchange:** the receiver holds a copy or derivative (`INFO` §4.24) unless ownership is explicitly reassigned through governance. A copy cites its source; a derivative preserves its relationship to the source.
- **Copies and derivatives** are labeled as such and are non-authoritative unless designated authoritative through change control (`INFO` §6.4).
- **Conflicts** — where two sides present conflicting authoritative claims — are recorded as conflict records and escalated to the authority with jurisdiction (`DECISION_CONTROL_ARCHITECTURE.md` §7); ambiguity about which source is correct is itself a defect (Constitution §10).
- **Boundary decisions and source-of-truth determinations** produced when an interface resolves an ownership question are preserved as the records defined in `INFO` §4.20 and §4.21; boundary is resolved before source of truth (`INFO` §6.3).
- **Duplication and silent divergence** are prevented by the single-owner rule: a fact appearing on both sides without one designated owner is a defect, tracked and resolved, not tolerated.

## 9. Interface Failure and Escalation

Failures are defined here as architectural categories, not operational incidents. Each is recorded and escalated per the control view (`DECISION_CONTROL_ARCHITECTURE.md` §7); none is silently resolved.

- **Missing required information** — an interface is asked to carry an object that is absent or incomplete. The exchange does not proceed on assumption; the gap is recorded.
- **Ambiguous ownership** — the authoritative owner of an exchanged fact cannot be determined. Resolved through a boundary/source-of-truth determination before the fact is treated as authoritative.
- **Unauthorized external action** — an outward effect is attempted without passing the External-Action Authorization Gate. The effect is blocked and recorded as a control violation.
- **Conflicting authoritative records** — two sides hold records that disagree, each claiming authority. Recorded as a conflict and escalated; one is designated authoritative, the other updated, deprecated, or removed.
- **Broken knowledge deposit** — a deposit fails to preserve the required information object, or a retrieval draws on a diverged derivative. Recorded as a preservation defect.
- **Rejected or incomplete handoff** — an interface exchange is declined or only partially completed. The incomplete state is preserved, not papered over, and routed to the appropriate authority.

## 10. Scope Boundaries

### 10.1 What Belongs in This Document

This document owns: durable interface categories; the studio↔product interface definitions; the architectural relationships among internal views; the external-effect constraint; and interface-level ownership, failure, and escalation rules.

### 10.2 What Belongs in `SYSTEM_CONTEXT.md`

The context view owns the boundary, the actors, and the naming of the boundary crossings. This document details those crossings; it does not redefine the boundary or the actors.

### 10.3 What Belongs in `CAPABILITY_DOMAIN_MAP.md`

The capability view owns the capabilities and their dependencies. This document connects capabilities through interfaces; it does not redefine them.

### 10.4 What Belongs in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`

The information view owns the information objects, their ownership, and their lifecycle. This document moves those objects across interfaces; it does not define them.

### 10.5 What Belongs in `HUMAN_AGENT_OPERATING_MODEL.md`

The operating model owns the human and agent role categories. This document connects those roles through interfaces; it does not define the roles.

### 10.6 What Belongs in `DECISION_CONTROL_ARCHITECTURE.md`

The control view owns the authorities, gates, and escalation mechanics. This document routes exchanges through those gates and references that escalation; it does not define the authorities or gates.

### 10.7 What Belongs in Implementation and Product Repositories

Implementation owns the mechanism of every interface — the tools, protocols, formats, channels, sequencing, and automation — and product repositories own their internal integration. This document defines the interfaces those implementations must conform to; it does not define them.

## 11. Known Unknowns

The following are explicitly unresolved and must be established by audit before this integration view can be marked [CURRENT]. They are recorded as known unknowns, not assumptions:

- Which interfaces currently exist in practice, and whether they carry defined information objects or undocumented assumptions.
- Whether current exchanges preserve single authoritative ownership, or whether facts are duplicated across sides without one owner.
- Whether product repositories currently exist and connect to VSOS only through the five studio-level interfaces, or through undocumented paths.
- Whether any current outward-facing effect bypasses the External-Action Authorization Gate.
- Whether current knowledge deposits and retrievals preserve the required information objects.
- Whether current copies and derivatives are labeled and cite their sources.
- Where interface ownership, boundary, or source of truth is currently ambiguous or blurred.
- Whether current handoffs record and escalate failure, or resolve it silently.

Each of these feeds the audit that precedes any redesign (preservation before replacement, Constitution §9).

---

*Draft v0.1. Realizes the integration view of the VSOS architecture. Subordinate to the Constitution; governed by `ARCHITECTURE_OVERVIEW.md`. Amendable only through change control. All interfaces are target architecture until audited; existing integrations remain unknown, and no interface bypasses human authority.*
