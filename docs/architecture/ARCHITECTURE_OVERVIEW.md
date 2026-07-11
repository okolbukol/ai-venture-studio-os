# VSOS Architecture Overview

**Status:** Draft v0.1
**Type:** Architecture — foundational
**Precedence:** Subordinate to the Constitution. Governs the architecture section (`docs/architecture/`).

## Preamble

This document is the entry point to the architecture of the Venture Studio Operating System (VSOS). It defines what the architecture is for, the constraints it inherits from the Constitution, the views used to describe it, the documents that compose it, and how it is governed and read.

It does not restate the Constitution. Where a rule already lives there, this document references it by section rather than repeating it.

---

## 1. Purpose of the VSOS Architecture

The architecture describes the **durable structure** of the studio: what the studio must be able to do, where its information lives, how work is divided between humans and agents, how authority flows, and how the parts connect. It is the stable frame that specific implementations are built onto.

**Architecture is not implementation.** The two are kept deliberately separate:

- **Architecture** — the slow-changing structure: capabilities, boundaries, information objects, roles, control points, interfaces. It answers *what*, *where*, *who owns it*, and *how the parts connect*.
- **Implementation** — the fast-changing realization: specific agents, workflows, code, templates, tools, and vendors. It answers *how, exactly, right now*.

Architecture changes rarely and only through change control. Implementation is expected to change often beneath a stable architecture. A change to a tool or an agent is not an architecture change; a change to a capability, boundary, or interface is.

This document is also not the Constitution. The Constitution sets studio-level principles and authority; the architecture translates those into structural constraints and describes the system they govern.

## 2. Architecture Principles

These are the constraints the architecture inherits from the Constitution, expressed as rules on how the architecture itself is built. Each binds every document in this section and everything implemented beneath it. Each traces to a constitutional source.

1. **Architecture over implementation.** The architecture is expressed independently of any specific agent, workflow, tool, or vendor. Implementation realizes the architecture and may change without changing it. *(Constitution §3.3)*
2. **Understanding precedes automation.** Nothing is built or automated before the capability it serves is defined here and reconciled with audited reality. The architecture is the understanding that must exist first. *(§3.4, §13)*
3. **No personal dependency.** The architecture is described in terms of capabilities, roles, and interfaces — never named individuals. A structure that works only because a particular person operates it is an architectural defect. *(§3.5)*
4. **One authoritative source per concern.** Each architectural concern is described in exactly one document. The others reference it; they do not restate it. Architecture-wide principles live only in this overview. *(§10)*
5. **Truth over invention.** The architecture records only what is known or explicitly defined as intended structure. Anything not yet audited is marked as unknown or target-state — never invented, never assumed into existence. *(§4)*
6. **Preservation before replacement.** The architecture describes intended structure, but existing systems are audited and mapped into it, and preserved where valuable, before any redesign. The architecture does not license rewrites. *(§9)*
7. **Control is architectural.** Human-authority checkpoints, product-lifecycle gates, and the Audit → Design → Approval → Implementation change process are first-class elements of the architecture, not implementation details. No downstream design may remove or bypass them. *(§5, §6, §7, §13)*
8. **Concision.** Architecture documents stay minimal and readable. Detail that belongs to implementation is pushed down, not absorbed here. *(§3.10)*

## 3. Architecture Views

VSOS is described through a small set of **views** — perspectives that each answer one question about the system. Every substantive view is realized by exactly one document (Section 4). This overview provides the governing view that ties them together.

- **Context view** — What is inside VSOS versus outside it, and who the actors are. *(Answers: where is the boundary?)*
- **Capability view** — The durable functions the studio must perform. *(Answers: what must the studio be able to do?)*
- **Information & knowledge view** — The objects the studio produces, where each authoritatively lives, and how knowledge flows and compounds. *(Answers: what information exists and where does it belong?)*
- **Operating-model view** — How work is allocated between human roles and AI agent roles across the capabilities. *(Answers: who or what performs the work?)*
- **Control view** — How authority, lifecycle gates, and change control flow through the system. *(Answers: how is the system governed in motion?)*
- **Integration view** — How capabilities connect to each other and to the outside world. *(Answers: where are the seams?)*

The views are complementary, not competing. A single reality — the studio — is described from several angles; the views must remain mutually consistent, and any conflict between them is a defect resolved through change control.

## 4. The Architecture Document Set

Seven documents compose this section. Each realizes one view; together, once individually approved, they form the complete architecture. They are ordered as a dependency chain — each builds on the ones before it.

1. **ARCHITECTURE_OVERVIEW.md** *(this document — governing view)* — Purpose, principles, views, document map, and governance of the architecture section.
2. **SYSTEM_CONTEXT.md** *(context view)* — Fixes the boundary of VSOS and identifies its actors and external touchpoints.
3. **CAPABILITY_DOMAIN_MAP.md** *(capability view)* — Decomposes the studio into its durable capabilities and domains, within the boundary set by (2).
4. **INFORMATION_KNOWLEDGE_ARCHITECTURE.md** *(information & knowledge view)* — Defines the information objects the capabilities in (3) produce, their authoritative homes, and how knowledge compounds.
5. **HUMAN_AGENT_OPERATING_MODEL.md** *(operating-model view)* — Defines how human roles and agent roles are allocated across the capabilities in (3).
6. **DECISION_CONTROL_ARCHITECTURE.md** *(control view)* — Defines how authority, lifecycle gates, and change control run across the whole system.
7. **INTEGRATION_INTERFACE_ARCHITECTURE.md** *(integration view)* — Defines the interfaces between the capabilities in (3) and to the outside, including the studio↔product interfaces.

Documents (2)–(7) describe the architecture; this document (1) governs how they are written, related, and changed. No document restates another; each links to the authoritative source for anything outside its own concern.

## 5. Architecture Governance and Change

Architecture is governed by the same discipline as the rest of the studio, specialized to this section.

- **Change process.** Every architecture change follows **Audit → Design → Approval → Implementation** (Constitution §13). Existing structure is audited, the change is designed with trade-offs and alternatives, a human authorized for architecture approves it, and only then is it recorded.
- **Decision records.** Consequential architecture decisions are recorded per Constitution §8 — the decision, its rationale, alternatives considered, and revisit conditions — so the reasoning survives the decision.
- **Single source of truth.** This repository is the single authoritative source for studio-level architecture (Constitution §10). Architecture stated anywhere else is a copy and is non-authoritative.
- **Versioning.** Architecture documents are versioned. Changes that alter a boundary, capability, information object, control point, or interface are architecture changes and are version-recorded; edits that only clarify wording are not.
- **Drift and reconciliation.** Where audited reality conflicts with what a document states, the conflict is not silently edited away and is not ignored. It is raised through the change process, which decides whether reality or the architecture is corrected.

## 6. How to Use This Section

- **Read in order.** The documents form a dependency chain (Section 4). Read the overview first, then follow the sequence; later documents assume the boundary and capabilities established by earlier ones.
- **Treat it as a constraint, not a suggestion.** Implementation — agents, workflows, code, tools — must conform to this architecture. Where implementation cannot conform, the architecture is changed through change control, not quietly diverged from.
- **Distinguish target from current.** Unless a document explicitly marks a section as audited-and-current, treat it as intended structure. Existing products and systems are described here only after they have been audited; until then they are referenced as unknown, not assumed.
- **When you find drift, route it.** If reality and a document disagree, or two documents disagree, raise it through the change process rather than editing in place. Consistency across the views is a property the architecture must preserve.

---

*Draft v0.1. Subordinate to the Constitution. Amendable only through the change-control process in Constitution §13, specialized in Section 5 above. Kept intentionally concise; implementation detail belongs below the architecture, not within it.*
