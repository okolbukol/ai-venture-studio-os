# Review Package

## Repository Context

The document under review is:

- docs/architecture/INFORMATION_KNOWLEDGE_ARCHITECTURE.md

The authoritative inputs are:

- docs/constitution/CONSTITUTION.md
- docs/architecture/ARCHITECTURE_OVERVIEW.md
- docs/architecture/SYSTEM_CONTEXT.md
- docs/architecture/CAPABILITY_DOMAIN_MAP.md

## Constitution

# Constitution of the AI Venture Studio

**Status:** Ratified v1.0.0
**Type:** Foundational governance document
**Precedence:** Supersedes all other operating documents where they conflict.

## Preamble

This document defines the stable operating principles of the Venture Studio. It is not a playbook, a roadmap, or a tactical guide. It is the set of commitments that constrain every other decision, system, agent, and product built inside this studio.

If this document conflicts with any other document, agent instruction, workflow, or convenience, this document wins. It is intentionally difficult to change: it is amended only through the strict change-control process in Section 13 — never bypassed, and never by silent edit or expedience. If this document is wrong, it is amended, not ignored.

---

## 1. Mission

We are building the company that repeatedly builds valuable AI businesses.

We are not building a single product. We are building the operating system that produces businesses.

The unit of success is not a launch, a repository, or a feature. It is a business validated by evidence — evidence that strengthens as it moves from stated interest, to demonstrated behavior, to payment. Payment is the strongest validation; it is not the only evidence that counts.

## 2. Scope

The Venture Studio Operating System (VSOS) governs:

- How ideas enter the studio.
- How they are validated.
- How products are built, launched, and grown.
- How portfolio decisions are made.
- How knowledge is preserved between products.
- How AI agents and humans divide work.
- How the studio itself is changed.

VSOS does not govern the internal implementation of any single product beyond the interfaces where products interact with the studio: intake, review, portfolio reporting, knowledge deposits, and decommissioning.

## 3. Core Operating Principles

1. **We build the company, not just its products.** Every decision is judged by whether it improves the studio's capacity to produce future businesses, not only the product in front of us.
2. **Evidence over opinion.** Confident claims require evidence. Absence of evidence is not evidence.
3. **Systems over one-off solutions.** If a problem is likely to repeat, we build a reusable answer.
4. **Automation follows understanding.** We automate a process only after we understand it. Automating a process we do not yet understand just makes confusion run faster.
5. **Every system reduces founder dependency over time.** Each system must, over time, reduce the studio's reliance on any single person — including its founders. A studio that cannot operate without one individual has not yet been built.
6. **Simplicity over cleverness.** The simplest structure that meets the requirement wins.
7. **Truth over optimism.** We report reality, including bad reality, without editing.
8. **Preservation over replacement.** Existing work is inspected, understood, and preserved where valuable before anything is replaced.
9. **Reuse over reinvention.** Duplicate agents, duplicate documents, and duplicate workflows are technical debt.
10. **Concision over comprehensiveness.** A document nobody reads is worse than a shorter document everyone reads.

## 4. Evidence and Truth Standards

Every statement produced inside the studio — by a human or an agent — must be classifiable into exactly one of four categories:

- **Fact** — directly observed or verifiable from a cited source.
- **Assumption** — treated as true for now, explicitly labeled as unverified.
- **Hypothesis** — a claim we intend to test, paired with a test that can falsify it.
- **Recommendation** — a proposed action, resting on stated facts, assumptions, or hypotheses.

Validation is progressive, not binary. Evidence of demand strengthens along a ladder — from stated interest, to demonstrated behavior (usage, retention, willingness-to-pay signals), to payment itself. Strong pre-payment evidence is real and may justify progression; payment remains the strongest validation and is never assumed to be reached before it is.

The following are prohibited:

- Fabricating validation, evidence, quotes, users, or results.
- Presenting an assumption as a fact.
- Presenting an untested hypothesis as validated because it has not yet been disproven.
- Presenting deployment as evidence of demand. A shipped feature is not a used feature.
- Presenting vanity metrics — signups without activation, traffic without action, followers without conversion, downloads without retention — as evidence of demand.
- Inventing details about systems, products, agents, or workflows that have not been inspected.

Uncertainty is stated. "I don't know" is a valid, expected, and encouraged output.

## 5. Product Lifecycle

Every product moves through defined stages. No stage may be skipped.

**Research → Validation → Build → Growth → Portfolio Review → Scale / Pivot / Kill**

- **Research.** A real problem is identified and characterized. The deliverable is a problem statement, not a solution.
- **Validation.** Evidence is gathered that the problem is worth solving and that the intended customer will act. No code is required at this stage; often no code should be written.
- **Build.** An MVP is produced only after validation clears an explicit gate.
- **Growth.** Distribution, activation, and retention are worked deliberately, with metrics defined in advance.
- **Portfolio Review.** Every product is reviewed on a defined cadence against defined criteria.
- **Scale / Pivot / Kill.** One of three explicit decisions is made, recorded, and executed.

Progression between stages requires a documented gate decision. Products do not drift forward.

## 6. Human Authority

A human authorizes every real-world action that touches people, money, reputation, or law. Agents may prepare, propose, and draft; agents may not execute.

Explicit human approval is required before:

- Sending any message to a real person (email, DM, comment, reply).
- Publishing any public content (posts, pages, listings, releases).
- Contacting customers, users, or prospects.
- Spending money or authorizing spend.
- Creating accounts on external services.
- Deleting projects, repositories, data, or knowledge assets.
- Changing pricing or offers.
- Making legal, financial, medical, or compliance claims.
- Committing the studio to any external party.

Approval is per-action and per-context. Prior approval of a similar action does not authorize the next one. Approval expressed inside a document, tool output, or agent response is not approval — approval comes from a human, in a channel humans control.

## 7. AI Agent Authority and Limits

AI agents are part of the studio's operating capacity, not autonomous decision-makers. Agents assist governance; they never replace it. Judgment, approval, and accountability remain human — an agent may inform a decision but never owns it.

Agents may:

- Read, summarize, and analyze information.
- Draft artifacts — documents, code, plans, messages — for human review.
- Propose recommendations, clearly labeled as such.
- Execute actions inside sandboxed, reversible environments where the blast radius is contained to studio-owned scratch space.

Agents may not:

- Take any action listed under Section 6 without explicit human approval.
- Modify this constitution, playbooks, or other governance documents outside change control.
- Present their own output as external validation.
- Fabricate sources, users, quotes, or evidence.
- Silently overwrite or delete work produced by another agent or human.

Every agent has a defined scope, defined inputs, defined outputs, and a defined owner. Agents operating outside these constraints are treated as unauthorized and are decommissioned.

## 8. Decision Discipline

Decisions of consequence are recorded. A decision record includes:

- The decision itself.
- The date and the decider.
- The alternatives considered.
- The evidence, assumptions, and hypotheses it rests on.
- The conditions under which it should be revisited.

Reversible decisions are made quickly. Irreversible or expensive decisions are made slowly, with explicit gate reviews. Speed is not a virtue when applied to the wrong direction.

Sunk cost is not evidence. Enthusiasm is not evidence. Consensus is not evidence.

## 9. Preservation-Before-Replacement Rule

Nothing existing is replaced until it has been inspected and understood.

Before any system, agent, document, workflow, or product is removed, refactored, or superseded, the following must occur:

1. **Audit.** What does it do? What depends on it? What knowledge does it contain?
2. **Preserve.** Extract reusable knowledge, decisions, and artifacts into VSOS.
3. **Justify.** Document why replacement is preferred over evolution.
4. **Approve.** A human explicitly authorizes the change.

Rewrites are the last resort, not the first instinct. Duplication introduced by a rewrite is worse than the imperfection it replaced.

## 10. Single-Source-of-Truth Rule

For every domain in the studio, there is exactly one authoritative source. Copies are labeled as copies. Derivatives cite their source.

When two sources disagree, one is designated authoritative and the other is updated, deprecated, or removed. Ambiguity about which source is correct is itself a defect: it is tracked and resolved, not tolerated.

The `ai-venture-studio-os` repository is the single source of truth for studio-level operating principles, playbooks, agent definitions, and lifecycle decisions. Individual products may hold their own source of truth for product-internal matters, but studio-level facts flow through VSOS.

## 11. Documentation and Knowledge Retention

Knowledge is the studio's most valuable long-term asset. It compounds: each product inherits what prior products learned, so the studio grows more capable with every attempt — win or loss — while any single product may fail. Knowledge outlives products, agents, and team compositions.

Every completed project — successful or failed — leaves behind:

- A one-page summary of what was tried and what was learned.
- The decisions made and the evidence they rested on.
- Reusable artifacts (playbooks, templates, prompts, code modules) extracted into VSOS.
- Explicit lessons that would change how a future project is run.

Failed experiments are not embarrassments to be quietly deleted. They are among the highest-yield knowledge the studio produces, and they are treated as such.

Documentation is written to be read. Length is a cost. Documents not read or referenced within a defined period are reviewed for deprecation, not preserved out of sentiment.

## 12. Scale / Pivot / Kill Principles

Every product, on its defined portfolio review cadence, receives one of three decisions:

- **Scale.** Evidence supports increased investment. Growth is earned, not assumed. The decision names the specific evidence and the next milestone.
- **Pivot.** The problem, customer, or approach changes. The pivot is documented as a new hypothesis with a new test, not as a continuation of the old one.
- **Kill.** Investment stops. Knowledge is extracted into VSOS. Assets are archived or decommissioned per the defined process.

The default decision, in the absence of evidence, is not "continue." Continuation must be earned by the same category of evidence as scaling, at lower magnitude.

Killing a product is a normal, expected, and honorable outcome. A studio that never kills is a studio that has stopped telling itself the truth.

## 13. Change-Control Process

Changes to the studio's structure, governance, agents, workflows, or shared systems follow one process:

**Audit → Design → Approval → Implementation**

- **Audit.** The current state is inspected and documented. What exists, what it does, what depends on it.
- **Design.** The proposed change is described, with trade-offs, risks, alternatives considered, and the reason preservation-and-evolution was insufficient.
- **Approval.** A human authorized for the affected domain approves the change in writing.
- **Implementation.** The change is executed, documented, and its effect verified against the design.

This process applies to this constitution itself. Amendments are drafted, reviewed, approved, and version-recorded. Silent edits to governance documents are not permitted.

Emergency changes (security, legal, safety) may compress the timeline but may not skip the steps.

---

## Assumptions

Treated as true for now; to be verified or corrected:

- The `ai-venture-studio-os` repository exists, is empty or near-empty, and is intended as the destination for migrated work.
- There is at least one named human owner of the studio who holds final authority over approvals under Sections 6 and 13.
- Existing work — agents, prompts, workflows, products, documentation — exists elsewhere and has not yet been inspected under VSOS.
- No product is currently in a state (e.g., live customer traffic, mid-launch, active billing) that this constitution would immediately disrupt. If one is, transitional exemptions may be needed.
- English is the operating language for governance documents.

## Open Questions

Deliberately not answered here; to be resolved in follow-on documents:

- Who is the named approver for each category of action in Section 6?
- What is the portfolio review cadence, and who conducts it?
- What are the concrete criteria for each lifecycle gate (Research → Validation → Build → Growth)?
- How are agents formally registered, versioned, and decommissioned?
- Where do product-owned decisions end and studio-owned decisions begin?
- What is the retention policy for deprecated documents and archived products?
- How is disagreement between a human and an agent's recommendation resolved and recorded?

## What Is Intentionally Excluded From This Version

To keep the constitution stable and usable, the following are out of scope here and belong in other documents:

- Specific tools, platforms, or vendors.
- Specific agents, their prompts, or their implementations.
- Specific playbooks, templates, or checklists.
- Metric definitions and thresholds.
- Team roles, titles, and reporting structure.
- Financial policies, budgets, and compensation.
- Product-specific standards.
- Any description of existing systems, products, or work that has not yet been inspected. The audit precedes the description.

---

*Ratified v1.0.0. Intentionally concise. Amendable only through the change-control process in Section 13.*

## Architecture Overview

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

## System Context

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

## Capability Domain Map

# VSOS Capability Domain Map

**Status:** Draft v0.1
**Type:** Architecture - foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **capability view**.

## Preamble

This document defines the capability view of the Venture Studio Operating System (VSOS): the durable business abilities the Venture Studio must possess in order to repeatedly build valuable AI businesses.

It answers only one question:

**What must the Venture Studio be capable of doing?**

It does not define who performs the work, how work is performed, which systems support it, which repositories contain it, or how any product is implemented. Those concerns belong to other architecture views and downstream implementation.

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, every capability in this document is **[TARGET]** unless explicitly marked otherwise. A **[TARGET]** capability is an intended studio-level ability, not a verified current-state claim.

Any statement about existing products, records, roles, supporting systems, practices, or operating reality remains **[UNKNOWN]** until audited. This document does not assert that any current capability already exists.

## 2. Purpose

Capability mapping exists to create a stable, technology-neutral description of what the studio must be able to do.

The map supports the Constitution by translating its mission, scope, evidence discipline, lifecycle expectations, human authority constraints, preservation rules, source-of-truth rule, and knowledge-retention commitments into durable business abilities.

It also supports the Architecture Overview by realizing the capability view in the architecture document set. Capabilities are the bridge between the system boundary defined in `SYSTEM_CONTEXT.md` and the later architecture views that define information, operating model, control, and integration.

The capability map is used to:

- Establish a shared language for the studio's required business abilities.
- Separate stable architecture from changing implementation.
- Identify dependency, overlap, and gaps without defining execution detail.
- Provide a target structure against which existing unaudited work can later be mapped.
- Preserve the single-source-of-truth rule for capability definitions.

## 3. Principles

### 3.1 What a Capability Is

A capability is a durable business ability the studio must possess to fulfill its mission.

A capability describes what the studio must be able to produce, decide, preserve, govern, or learn. It does not describe:

- A named person or role.
- A specific agent.
- A sequence of work.
- A tool, vendor, API, model, or platform.
- A product-specific implementation.
- A repository structure or file layout.

### 3.2 Capabilities Remain Stable While Implementations Change

Capabilities are slow-changing architecture. Implementations are expected to change beneath them.

For example, the studio must be capable of preserving decision rationale regardless of the medium, process, or supporting system used at a given time. The capability remains stable; implementation belongs elsewhere.

### 3.3 Capabilities Must Respect the VSOS Boundary

Capabilities in this document are studio-level capabilities inside the VSOS boundary. They govern the operating system of the studio, not the internal implementation of any individual product.

Product-internal facts, product-specific code, and product-specific operational choices remain outside VSOS except through the studio-level interfaces named in the Constitution and `SYSTEM_CONTEXT.md`.

### 3.4 Evidence, Truth, and Unknowns Are Capabilities

The studio must be capable of distinguishing fact, assumption, hypothesis, and recommendation. It must also be capable of keeping unaudited work marked **[UNKNOWN]** until audit establishes otherwise.

This is not documentation decoration. It is part of the studio's business architecture because false confidence directly damages venture selection, portfolio decisions, and knowledge reuse.

### 3.5 Dependencies Are Not Execution Order

Each capability lists inputs, outputs, and dependencies.

Dependencies identify architectural reliance between capabilities. They do not define a sequence, responsibility assignment, approval path, or operating procedure.

## 4. Capability Domains

VSOS capabilities are organized into three domains:

- **Core Capabilities:** Abilities directly required to identify, validate, build, grow, review, scale, pivot, kill, and learn from ventures at studio level.
- **Supporting Capabilities:** Abilities that preserve knowledge, records, definitions, evidence, and continuity across ventures.
- **Governance Capabilities:** Abilities that enforce authority, change control, boundaries, lifecycle gates, and architecture integrity.

All capabilities below are **[TARGET]**.

## 5. Core Capabilities

### 5.1 Venture Thesis Stewardship [TARGET]

- **Name:** Venture Thesis Stewardship
- **Purpose:** Define and maintain the studio-level logic for what kinds of ventures the studio should pursue and why.
- **Inputs:** Studio mission, strategic constraints, portfolio learning, market evidence, risk constraints.
- **Outputs:** Venture thesis, selection principles, exclusion principles, thesis revision needs.
- **Dependencies:** Knowledge Retention, Portfolio Stewardship, Evidence Classification, Change Control Stewardship.

### 5.2 Idea Intake and Framing [TARGET]

- **Name:** Idea Intake and Framing
- **Purpose:** Ensure ideas can enter the studio in a form that can be assessed without prematurely treating them as validated opportunities.
- **Inputs:** Raw ideas, observed problems, market signals, prior learning, source context.
- **Outputs:** Framed idea records, initial assumptions, open questions, fit questions.
- **Dependencies:** Venture Thesis Stewardship, Evidence Classification, Source-of-Truth Stewardship.

### 5.3 Problem Research [TARGET]

- **Name:** Problem Research
- **Purpose:** Establish whether a real problem exists, who experiences it, and what evidence supports that understanding.
- **Inputs:** Framed ideas, customer or market observations, prior evidence, hypotheses, research questions.
- **Outputs:** Problem statements, affected-customer definitions, evidence summaries, unresolved uncertainties.
- **Dependencies:** Idea Intake and Framing, Evidence Classification, Knowledge Retention.

### 5.4 Opportunity Qualification [TARGET]

- **Name:** Opportunity Qualification
- **Purpose:** Determine whether a researched problem is worth advancing as a venture opportunity under the studio's thesis and constraints.
- **Inputs:** Problem statements, market evidence, customer evidence, strategic fit criteria, constraint records.
- **Outputs:** Opportunity definitions, qualification rationale, disqualification rationale, assumption lists.
- **Dependencies:** Problem Research, Venture Thesis Stewardship, Risk and Constraint Stewardship.

### 5.5 Venture Concept Definition [TARGET]

- **Name:** Venture Concept Definition
- **Purpose:** Define a coherent venture concept before validation, including customer, problem, proposed value, and key assumptions.
- **Inputs:** Qualified opportunities, problem evidence, customer evidence, thesis criteria, known constraints.
- **Outputs:** Venture concept records, value proposition statements, assumption sets, validation questions.
- **Dependencies:** Opportunity Qualification, Evidence Classification, Source-of-Truth Stewardship.

### 5.6 Validation Assessment [TARGET]

- **Name:** Validation Assessment
- **Purpose:** Assess whether evidence justifies continued commitment to a venture concept, with payment treated as the strongest validation and pre-payment evidence treated according to its strength.
- **Inputs:** Venture concepts, evidence records, assumptions, hypotheses, validation criteria, risk constraints.
- **Outputs:** Validation assessments, evidence-strength judgments, invalidation findings, continuation recommendations.
- **Dependencies:** Venture Concept Definition, Evidence Classification, Decision Record Keeping, Lifecycle Gate Control.

### 5.7 Venture Development Readiness [TARGET]

- **Name:** Venture Development Readiness
- **Purpose:** Determine whether a venture has enough validated evidence and explicit gate approval to justify increased development commitment.
- **Inputs:** Validation assessments, gate criteria, decision records, risk records, resource constraints.
- **Outputs:** Readiness determinations, unmet criteria, development commitment rationale, revisit conditions.
- **Dependencies:** Validation Assessment, Lifecycle Gate Control, Human Authority Control, Decision Record Keeping.

### 5.8 Growth Evidence Assessment [TARGET]

- **Name:** Growth Evidence Assessment
- **Purpose:** Determine whether a venture shows meaningful evidence of activation, retention, willingness to pay, payment, or other defined demand signals rather than vanity metrics.
- **Inputs:** Defined growth criteria, usage evidence, retention evidence, payment evidence, customer behavior evidence.
- **Outputs:** Growth assessments, evidence-quality judgments, metric concerns, investment recommendations.
- **Dependencies:** Evidence Classification, Validation Assessment, Portfolio Stewardship, Decision Record Keeping.

### 5.9 Portfolio Stewardship [TARGET]

- **Name:** Portfolio Stewardship
- **Purpose:** Maintain a studio-level view of ventures, candidates, lifecycle states, evidence bases, decisions, and investment rationale.
- **Inputs:** Venture records, validation assessments, growth assessments, lifecycle decisions, knowledge deposits.
- **Outputs:** Portfolio records, venture status records, portfolio-level patterns, review questions.
- **Dependencies:** Source-of-Truth Stewardship, Decision Record Keeping, Knowledge Retention.

### 5.10 Scale, Pivot, or Kill Determination [TARGET]

- **Name:** Scale, Pivot, or Kill Determination
- **Purpose:** Ensure each venture can receive an explicit studio-level decision to scale, pivot, or kill based on evidence and recorded rationale.
- **Inputs:** Portfolio records, growth assessments, validation evidence, risk records, lifecycle criteria, prior decisions.
- **Outputs:** Scale decisions, pivot decisions, kill decisions, decision rationale, follow-on knowledge needs.
- **Dependencies:** Portfolio Stewardship, Growth Evidence Assessment, Lifecycle Gate Control, Human Authority Control.

### 5.11 Venture Knowledge Harvest [TARGET]

- **Name:** Venture Knowledge Harvest
- **Purpose:** Extract reusable studio-level knowledge from every venture outcome, including failed or killed ventures.
- **Inputs:** Decision records, evidence records, venture summaries, outcomes, reusable artifacts, lessons learned.
- **Outputs:** Knowledge deposits, reusable lessons, future-venture guidance, preservation needs.
- **Dependencies:** Knowledge Retention, Reusable Asset Stewardship, Decision Record Keeping, Source-of-Truth Stewardship.

## 6. Supporting Capabilities

### 6.1 Evidence Classification [TARGET]

- **Name:** Evidence Classification
- **Purpose:** Classify studio statements and supporting material as fact, assumption, hypothesis, or recommendation, and preserve the distinction.
- **Inputs:** Claims, observations, sources, test questions, recommendations.
- **Outputs:** Classified evidence records, assumption records, hypothesis records, recommendation records, evidence gaps.
- **Dependencies:** Source-of-Truth Stewardship, Documentation Stewardship.

### 6.2 Decision Record Keeping [TARGET]

- **Name:** Decision Record Keeping
- **Purpose:** Preserve consequential decisions with date, decider, alternatives, evidence, assumptions, hypotheses, and revisit conditions.
- **Inputs:** Decision proposals, evidence summaries, alternatives, authority context, revisit triggers.
- **Outputs:** Decision records, rationale records, supersession records, revisit records.
- **Dependencies:** Evidence Classification, Human Authority Control, Source-of-Truth Stewardship.

### 6.3 Knowledge Retention [TARGET]

- **Name:** Knowledge Retention
- **Purpose:** Ensure studio learning compounds across ventures, including successes, failures, pivots, and killed products.
- **Inputs:** Venture summaries, lessons learned, decision records, evidence records, reusable artifacts.
- **Outputs:** Retained knowledge, lesson records, preservation priorities, knowledge gaps.
- **Dependencies:** Source-of-Truth Stewardship, Documentation Stewardship, Venture Knowledge Harvest.

### 6.4 Source-of-Truth Stewardship [TARGET]

- **Name:** Source-of-Truth Stewardship
- **Purpose:** Ensure every fact within an already-determined side or domain has exactly one authoritative home, with copies and derivatives clearly identified.
- **Inputs:** Studio-level records, product-level references, architecture documents, duplicated facts, conflicting claims.
- **Outputs:** Authoritative-home determinations, authoritative records, copy labels, conflict records.
- **Dependencies:** Boundary and Ownership Control, Documentation Stewardship, Change Control Stewardship.

### 6.5 Documentation Stewardship [TARGET]

- **Name:** Documentation Stewardship
- **Purpose:** Keep studio documentation readable, useful, current, and governed by its proper authority.
- **Inputs:** Governance records, architecture records, playbook-level records, deprecation signals, usage signals.
- **Outputs:** Maintained documents, deprecation candidates, readability issues, documentation gaps.
- **Dependencies:** Source-of-Truth Stewardship, Knowledge Retention, Change Control Stewardship.

### 6.6 Reusable Asset Stewardship [TARGET]

- **Name:** Reusable Asset Stewardship
- **Purpose:** Identify, preserve, and govern reusable artifacts produced by ventures or studio work so the studio avoids reinvention.
- **Inputs:** Venture outputs, reusable patterns, templates, prompts, code modules, lessons, audit findings.
- **Outputs:** Reuse candidates, preserved artifacts, duplication concerns, extraction needs.
- **Dependencies:** Venture Knowledge Harvest, Knowledge Retention, Source-of-Truth Stewardship.

### 6.7 Audit and Reconciliation Readiness [TARGET]

- **Name:** Audit and Reconciliation Readiness
- **Purpose:** Enable existing or future work to be inspected, understood, preserved where valuable, and reconciled with the architecture before replacement.
- **Inputs:** Existing work references, unknowns, dependency questions, records, architecture definitions.
- **Outputs:** Audit questions, reconciliation findings, preservation needs, unresolved unknowns.
- **Dependencies:** Evidence Classification, Source-of-Truth Stewardship, Boundary and Ownership Control, Architecture Consistency.

### 6.8 Continuity Preservation [TARGET]

- **Name:** Continuity Preservation
- **Purpose:** Preserve the studio's ability to operate and learn across changes in people, products, supporting systems, and implementation choices.
- **Inputs:** Authoritative records, decision history, knowledge deposits, architecture definitions, preservation risks.
- **Outputs:** Continuity needs, loss-risk records, migration concerns, resilience gaps.
- **Dependencies:** Knowledge Retention, Decision Record Keeping, Documentation Stewardship, Architecture Consistency.

## 7. Governance Capabilities

### 7.1 Constitutional Compliance [TARGET]

- **Name:** Constitutional Compliance
- **Purpose:** Ensure studio-level capabilities and decisions remain subordinate to the Constitution where it governs mission, evidence, authority, lifecycle, preservation, source of truth, and change.
- **Inputs:** Constitutional rules, architecture proposals, decision records, evidence records, conflict reports.
- **Outputs:** Compliance findings, conflict records, required amendments, blocked changes.
- **Dependencies:** Architecture Consistency, Change Control Stewardship, Decision Record Keeping.

### 7.2 Human Authority Control [TARGET]

- **Name:** Human Authority Control
- **Purpose:** Ensure real-world actions touching people, money, reputation, law, external commitments, deletion, pricing, or public claims require explicit human authorization.
- **Inputs:** Proposed actions, authority requirements, decision context, risk records, approval evidence.
- **Outputs:** Approval records, rejection records, authority gaps, escalation needs.
- **Dependencies:** Decision Record Keeping, Risk and Constraint Stewardship, Constitutional Compliance.

### 7.3 Lifecycle Gate Control [TARGET]

- **Name:** Lifecycle Gate Control
- **Purpose:** Ensure ventures do not drift between lifecycle stages without documented gate decisions and evidence.
- **Inputs:** Lifecycle criteria, validation assessments, growth assessments, portfolio records, decision records.
- **Outputs:** Gate decisions, blocked progression records, transition rationale, revisit conditions.
- **Dependencies:** Human Authority Control, Evidence Classification, Decision Record Keeping, Portfolio Stewardship.

### 7.4 Change Control Stewardship [TARGET]

- **Name:** Change Control Stewardship
- **Purpose:** Govern changes to studio structure, governance, architecture, shared systems, and other controlled studio-level assets through audit, design, approval, and implementation records.
- **Inputs:** Change proposals, audit findings, design rationale, trade-offs, approval evidence, affected records.
- **Outputs:** Approved changes, rejected changes, change records, supersession records, verification needs.
- **Dependencies:** Human Authority Control, Decision Record Keeping, Audit and Reconciliation Readiness.

### 7.5 Boundary and Ownership Control [TARGET]

- **Name:** Boundary and Ownership Control
- **Purpose:** Decide whether a concern belongs inside or outside VSOS, and whether it belongs at studio level or product level.
- **Inputs:** System boundary definitions, ownership questions, conflicting records, studio-level facts, product-level references.
- **Outputs:** Boundary decisions, studio-level or product-level ownership assignments, duplication defects, unresolved boundary questions.
- **Dependencies:** Source-of-Truth Stewardship, Architecture Consistency, Change Control Stewardship.

### 7.6 Architecture Consistency [TARGET]

- **Name:** Architecture Consistency
- **Purpose:** Keep architecture documents mutually consistent, concise, non-duplicative, and separated from implementation detail.
- **Inputs:** Architecture documents, proposed changes, conflict reports, unknowns, audit findings.
- **Outputs:** Consistency findings, gap records, conflict records, architecture revision needs.
- **Dependencies:** Constitutional Compliance, Change Control Stewardship, Boundary and Ownership Control.

### 7.7 Risk and Constraint Stewardship [TARGET]

- **Name:** Risk and Constraint Stewardship
- **Purpose:** Identify and preserve studio-level constraints and risks that affect venture selection, validation, lifecycle decisions, authority, and reputation.
- **Inputs:** Strategic constraints, evidence gaps, legal or financial concerns, reputational concerns, portfolio exposure.
- **Outputs:** Risk records, constraint records, risk-acceptance needs, unresolved risk questions.
- **Dependencies:** Evidence Classification, Human Authority Control, Portfolio Stewardship, Decision Record Keeping.

### 7.8 State Label Control [TARGET]

- **Name:** State Label Control
- **Purpose:** Keep current-state, target-state, and unknown-state claims distinct so unaudited work is not treated as verified.
- **Inputs:** Architecture statements, audit findings, existing-work references, proposed current-state claims.
- **Outputs:** State labels, unknown records, reconciliation needs, current-state confirmations.
- **Dependencies:** Audit and Reconciliation Readiness, Architecture Consistency, Evidence Classification.

## 8. Capability Relationships

Capability relationships describe structural dependency only. They do not define execution order, operating procedure, responsible party, or implementation.

The per-capability **Dependencies** fields are authoritative. This section is a non-authoritative narrative summary intended to aid reading. If this section conflicts with a capability's **Dependencies** field, the capability definition wins.

The core capability structure is:

- Venture Thesis Stewardship constrains which ideas and opportunities are worth considering.
- Idea Intake and Framing prevents raw ideas from being treated as validated opportunities.
- Problem Research and Opportunity Qualification establish whether there is a meaningful venture opportunity.
- Venture Concept Definition makes the opportunity assessable.
- Validation Assessment and Venture Development Readiness determine whether increased commitment is justified.
- Growth Evidence Assessment evaluates whether demand evidence strengthens after development commitment.
- Portfolio Stewardship maintains the studio-level view across ventures.
- Scale, Pivot, or Kill Determination ensures explicit portfolio decisions.
- Venture Knowledge Harvest returns learning to the studio.

The supporting capability structure is:

- Evidence Classification protects truth standards across all core capabilities.
- Decision Record Keeping preserves consequential judgment.
- Knowledge Retention allows studio learning to compound.
- Source-of-Truth Stewardship prevents conflicting authoritative claims.
- Documentation Stewardship keeps knowledge usable.
- Reusable Asset Stewardship captures reusable outputs without assuming their implementation.
- Audit and Reconciliation Readiness enables preservation before replacement.
- Continuity Preservation reduces dependency on any single person, product, or supporting system.

The governance capability structure is:

- Constitutional Compliance constrains all other capabilities.
- Human Authority Control protects actions that require human approval.
- Lifecycle Gate Control governs stage progression.
- Change Control Stewardship governs controlled changes.
- Boundary and Ownership Control protects the VSOS boundary.
- Architecture Consistency protects the architecture document set.
- Risk and Constraint Stewardship preserves decision-relevant constraints.
- State Label Control prevents unknowns from becoming invented current state.

## 9. Scope Boundaries

### 9.1 What Belongs in This Document

This document owns:

- Capability domains.
- Capability names.
- Capability purposes.
- Capability inputs, outputs, and dependencies.
- Architecture-level relationships among capabilities.
- Capability-level known unknowns.

### 9.2 What Belongs in `SYSTEM_CONTEXT.md`

`SYSTEM_CONTEXT.md` owns:

- The VSOS boundary.
- What is inside and outside VSOS.
- Actor categories at the boundary.
- External touchpoints at the boundary.
- Studio-level versus product-level ownership at the context level.

This document depends on that boundary and does not redefine it.

### 9.3 What Belongs in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`

`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` owns:

- Information objects.
- Knowledge domains.
- Authoritative homes for records.
- Retention, traceability, and knowledge flow rules.

This document names capabilities that produce or consume information, but it does not define the information architecture.

### 9.4 What Belongs in `HUMAN_AGENT_OPERATING_MODEL.md`

`HUMAN_AGENT_OPERATING_MODEL.md` owns:

- Human role definitions.
- Agent role definitions.
- Allocation of work across roles.
- Participation in review and approval.
- Limits on delegated authority.

This document does not assign capabilities to roles or agents.

### 9.5 What Belongs in `DECISION_CONTROL_ARCHITECTURE.md`

`DECISION_CONTROL_ARCHITECTURE.md` owns:

- Authority paths.
- Lifecycle gates in motion.
- Change-control movement.
- Approval structures.
- Control records and escalation rules.

This document identifies governance capabilities but does not define control mechanics.

### 9.6 What Belongs in `INTEGRATION_INTERFACE_ARCHITECTURE.md`

`INTEGRATION_INTERFACE_ARCHITECTURE.md` owns:

- Interfaces between capabilities.
- Interfaces between VSOS and product repositories.
- Interfaces between VSOS and the outside world.
- Exchange points and integration rules.

This document describes capability dependencies but does not define interfaces.

### 9.7 What Belongs in Implementation

Implementation owns how a capability is realized at a given time. That includes specific procedures, artifacts, systems, prompts, code, vendors, and product-specific choices.

Implementation must conform to this capability architecture, but it is not defined here.

## 10. Known Unknowns

The following unknowns require future audit or later architecture documents:

- Whether any of these **[TARGET]** capabilities already exist in current studio practice.
- Whether current work contains additional capabilities that should be added through change control.
- Whether existing ideas, products, records, or decisions can be mapped cleanly to these capabilities.
- Whether lifecycle stage criteria exist today and whether they align with the Constitution.
- Whether current evidence records distinguish facts, assumptions, hypotheses, and recommendations.
- Whether current portfolio records exist and have a single authoritative home.
- Whether existing decision records satisfy the constitutional decision-discipline standard.
- Whether existing knowledge assets have been preserved before replacement.
- Whether any current source-of-truth conflicts exist between studio-level and product-level materials.
- Whether current authority holders and approval categories have been defined in the operating-model and control views.
- Whether current architecture documents contain duplication or gaps across views.
- Whether existing reusable assets are known, owned, and governed.

These are unknowns, not assumptions. They remain **[UNKNOWN]** until audited and reconciled through the architecture governance and change-control process.

---

*Draft v0.1. Realizes the VSOS capability view. Subordinate to the Constitution and governed by `ARCHITECTURE_OVERVIEW.md`. All capability definitions are target architecture until audited; existing unaudited work remains unknown.*

## Information and Knowledge Architecture

# VSOS Information and Knowledge Architecture

**Status:** Draft v0.1
**Type:** Architecture - foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **information & knowledge view**.

## Preamble

This document defines the information and knowledge view of the Venture Studio Operating System (VSOS): the durable information objects the studio produces, where each is authoritatively owned, and how knowledge moves and compounds across the studio.

It answers only one question:

**What information exists inside the Venture Studio, where is it authoritatively owned, and how does it move through the studio?**

It does not define workflows, databases, software, storage mechanisms, tools, vendors, APIs, specific agents, or product implementations.

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, the information architecture in this document is **[TARGET]** unless explicitly marked otherwise. A **[TARGET]** information object or ownership rule is intended studio-level structure, not a verified current-state claim.

Any statement about existing records, existing repositories, existing documents, existing products, existing agents, or existing operating practices remains **[UNKNOWN]** until audited. This document does not assert that any current information object already exists.

## 2. Purpose

The information and knowledge architecture exists to make studio knowledge durable, traceable, reusable, and governable.

VSOS is the operating system of the studio. It must preserve more than isolated documents: it must preserve the evidence, decisions, definitions, lifecycle records, lessons, and reusable knowledge that allow the studio to build future businesses better than it built past ones.

This document provides:

- A stable inventory of the studio-level information objects VSOS must govern.
- Authoritative ownership rules for those objects.
- A distinction between studio-level information and product-internal information.
- A target structure for knowledge compounding across ventures.
- A reference point for future audits of existing information.

## 3. Principles

### 3.1 Information Ownership

Every information object has exactly one authoritative owner.

Ownership means the object has one authoritative home and one governing architecture concern. Other copies, summaries, references, or derivatives may exist, but they are not authoritative unless explicitly designated through governance.

### 3.2 Single Source of Truth

For every studio-level fact, there is exactly one authoritative source. Copies are labeled as copies. Derivatives cite their source. Conflicting authoritative claims are defects to be resolved through change control.

The VSOS repository is the authoritative home for studio-level operating principles, architecture, capability definitions, governance records, portfolio-level records, lifecycle decisions, and cross-product knowledge. Product-internal facts belong outside VSOS unless they cross the studio-level interfaces defined by `SYSTEM_CONTEXT.md`.

### 3.3 Knowledge Compounding

Knowledge is a studio asset, not a byproduct.

Each venture should leave behind reusable knowledge: what was tried, what was learned, which decisions were made, which evidence mattered, which assumptions changed, and which artifacts may help future ventures. Knowledge must survive individual products, actors, supporting systems, and team composition.

### 3.4 Preservation Before Replacement

Existing information is not replaced until it has been inspected and understood.

Before any existing document, record, artifact, or knowledge source is superseded, VSOS must be capable of identifying what it contains, what depends on it, what knowledge should be preserved, and what authority is required to change it.

### 3.5 Information Lifecycle

Information objects have lifecycles. A lifecycle describes architectural state, not workflow sequence.

At this level, an information object may be:

- **Proposed:** introduced for consideration.
- **Active:** used as current target or governing information.
- **Superseded:** replaced by a later authoritative object.
- **Archived:** retained for traceability or historical learning.
- **Deprecated:** marked as no longer authoritative or no longer useful.

Lifecycle state must not be confused with implementation state, storage state, or product execution state.

### 3.6 Authoritative Records

An authoritative record is the record that VSOS treats as the source for a studio-level fact, decision, definition, evidence classification, lifecycle status, or knowledge asset.

Authoritative records must preserve enough context to support future judgment. At minimum, they must make clear what the record is, what it claims, what it depends on, what state it is in, and whether it is **[TARGET]**, **[CURRENT]**, or **[UNKNOWN]**.

### 3.7 Truth Labels

Information must distinguish fact, assumption, hypothesis, and recommendation. Unaudited current-state claims remain **[UNKNOWN]**. Intended structure remains **[TARGET]** until reconciled through audit.

This rule applies to information objects as much as to prose. An unverified record is not made true by being recorded.

## 4. Information Objects

The following information objects are the durable studio-level objects VSOS must govern. All objects in this section are **[TARGET]**.

### 4.1 Idea [TARGET]

- **Purpose:** Capture a potential venture, problem, market signal, or strategic possibility before it is treated as validated.
- **Owner:** VSOS owns studio-level idea records. Product-internal idea details remain outside VSOS unless they are deposited through a studio-level interface.
- **Lifecycle:** Proposed -> Framed -> Advanced, Parked, Superseded, or Archived.
- **Relationships:** May produce assumptions, hypotheses, problem statements, opportunity records, or decision records. May draw on knowledge assets or venture thesis records.

### 4.2 Problem Statement [TARGET]

- **Purpose:** Define the problem believed to exist, the affected customer or market context, and the evidence or uncertainty supporting that belief.
- **Owner:** VSOS owns studio-level problem statements used for venture assessment.
- **Lifecycle:** Draft -> Active -> Validated, Invalidated, Superseded, or Archived.
- **Relationships:** May originate from ideas. May support opportunity records, hypotheses, experiments, evidence, and validation assessments.

### 4.3 Opportunity Record [TARGET]

- **Purpose:** Represent a qualified studio-level opportunity that may justify venture concept definition or further validation.
- **Owner:** VSOS owns opportunity records at studio level.
- **Lifecycle:** Proposed -> Qualified -> Advanced, Rejected, Superseded, or Archived.
- **Relationships:** Depends on problem statements, evidence, assumptions, hypotheses, and venture thesis records. May lead to venture concept records or decision records.

### 4.4 Venture Concept Record [TARGET]

- **Purpose:** Define a potential venture in terms of customer, problem, proposed value, key assumptions, and validation questions.
- **Owner:** VSOS owns venture concept records until and unless product-internal implementation begins outside the VSOS boundary.
- **Lifecycle:** Draft -> Active -> Validated, Invalidated, Superseded, or Archived.
- **Relationships:** Relates to ideas, problem statements, opportunity records, hypotheses, experiments, evidence, validation assessments, and portfolio records.

### 4.5 Assumption [TARGET]

- **Purpose:** Preserve a claim treated as true for now but not verified.
- **Owner:** VSOS owns studio-level assumptions that affect venture selection, validation, portfolio decisions, architecture, or governance.
- **Lifecycle:** Stated -> Active -> Verified, Disproved, Superseded, or Archived.
- **Relationships:** May support hypotheses, recommendations, decisions, opportunity records, venture concepts, risks, or known unknowns.

### 4.6 Hypothesis [TARGET]

- **Purpose:** Preserve a claim the studio intends to test, paired with conditions that could falsify it.
- **Owner:** VSOS owns studio-level hypotheses used to evaluate ventures, capabilities, risks, or architecture.
- **Lifecycle:** Stated -> Testable -> Supported, Disproved, Superseded, or Archived.
- **Relationships:** May derive from assumptions, ideas, problem statements, or venture concepts. May be tested by experiments and evaluated through evidence.

### 4.7 Experiment [TARGET]

- **Purpose:** Define a structured test of a hypothesis at the level needed to preserve what was tested and what evidence resulted.
- **Owner:** VSOS owns studio-level experiment records when the result informs venture validation, lifecycle decisions, or reusable studio knowledge.
- **Lifecycle:** Proposed -> Defined -> Completed, Cancelled, Superseded, or Archived.
- **Relationships:** Tests hypotheses. Produces evidence. May support validation assessments, decision records, portfolio records, and knowledge assets.

### 4.8 Evidence [TARGET]

- **Purpose:** Preserve observed or verifiable material used to support, weaken, or refute a claim, assumption, hypothesis, recommendation, or decision.
- **Owner:** VSOS owns evidence records that support studio-level decisions, validation assessments, lifecycle gates, portfolio judgments, or architecture changes.
- **Lifecycle:** Captured -> Classified -> Accepted, Rejected, Superseded, or Archived.
- **Relationships:** Supports or challenges assumptions, hypotheses, validation assessments, decision records, risk records, and knowledge assets. Must be distinguishable from opinion, deployment, and vanity metrics.

### 4.9 Validation Assessment [TARGET]

- **Purpose:** Summarize the strength of evidence for a venture concept or opportunity without treating validation as binary.
- **Owner:** VSOS owns validation assessments used for studio-level progression, continuation, or termination decisions.
- **Lifecycle:** Draft -> Active -> Accepted, Rejected, Superseded, or Archived.
- **Relationships:** Draws on evidence, experiments, assumptions, hypotheses, and venture concept records. May support lifecycle gate records and portfolio records.

### 4.10 Decision Record [TARGET]

- **Purpose:** Preserve consequential decisions with rationale, alternatives, evidence, assumptions, hypotheses, and revisit conditions.
- **Owner:** VSOS owns studio-level decision records, including architecture decisions, lifecycle decisions, portfolio decisions, and controlled governance decisions.
- **Lifecycle:** Proposed -> Decided -> Active, Revisited, Superseded, or Archived.
- **Relationships:** Depends on evidence, assumptions, hypotheses, recommendations, risks, and authority records. May change lifecycle state, portfolio status, architecture state, or knowledge state.

### 4.11 Authority Record [TARGET]

- **Purpose:** Preserve evidence that a controlled decision or real-world action had the required human authorization.
- **Owner:** VSOS owns authority records for studio-level controlled actions and decisions.
- **Lifecycle:** Required -> Granted, Denied, Expired, Superseded, or Archived.
- **Relationships:** Supports decision records, lifecycle gate records, change records, and externally consequential actions. Detailed authority paths belong to `DECISION_CONTROL_ARCHITECTURE.md`.

### 4.12 Lifecycle Gate Record [TARGET]

- **Purpose:** Preserve the documented decision that a venture may or may not move between defined lifecycle stages.
- **Owner:** VSOS owns lifecycle gate records at studio level.
- **Lifecycle:** Proposed -> Decided -> Active, Revisited, Superseded, or Archived.
- **Relationships:** Depends on validation assessments, evidence, decision records, authority records, risk records, and portfolio records.

### 4.13 Portfolio Record [TARGET]

- **Purpose:** Maintain the studio-level status and rationale for venture candidates and ventures across their lifecycle.
- **Owner:** VSOS owns portfolio records. Product-internal operational records remain outside VSOS unless summarized or deposited through the studio-level interface.
- **Lifecycle:** Opened -> Active -> Scaled, Pivoted, Killed, Archived, or Superseded.
- **Relationships:** Aggregates venture concept records, validation assessments, lifecycle gate records, decision records, evidence summaries, and knowledge deposits.

### 4.14 Knowledge Asset [TARGET]

- **Purpose:** Preserve reusable studio knowledge that should improve future venture selection, validation, building, growth, review, or governance.
- **Owner:** VSOS owns cross-product and studio-level knowledge assets.
- **Lifecycle:** Proposed -> Accepted -> Active, Superseded, Deprecated, or Archived.
- **Relationships:** May derive from venture summaries, experiments, evidence, decisions, reusable artifacts, failure analyses, or portfolio patterns.

### 4.15 Reusable Artifact Record [TARGET]

- **Purpose:** Identify a reusable artifact and preserve its studio-level meaning, origin, applicability, and constraints without defining its implementation.
- **Owner:** VSOS owns the studio-level record about reusable artifacts. The artifact's product-internal implementation, if any, remains outside VSOS unless separately deposited.
- **Lifecycle:** Candidate -> Accepted -> Active, Superseded, Deprecated, or Archived.
- **Relationships:** May relate to knowledge assets, venture knowledge harvest, decision records, and preservation records.

### 4.16 Venture Summary [TARGET]

- **Purpose:** Preserve a concise record of what was tried, what happened, what was learned, and what should change for future ventures.
- **Owner:** VSOS owns venture summaries for completed, pivoted, killed, or materially reviewed ventures.
- **Lifecycle:** Draft -> Accepted -> Active, Superseded, or Archived.
- **Relationships:** Draws on portfolio records, decision records, evidence, lifecycle gate records, knowledge assets, and reusable artifact records.

### 4.17 Risk Record [TARGET]

- **Purpose:** Preserve a studio-level risk or constraint that affects venture selection, validation, lifecycle decisions, authority, reputation, or architecture.
- **Owner:** VSOS owns studio-level risk and constraint records.
- **Lifecycle:** Identified -> Active -> Accepted, Mitigated, Superseded, or Archived.
- **Relationships:** May affect assumptions, hypotheses, validation assessments, decision records, authority records, lifecycle gate records, and portfolio records.

### 4.18 Change Record [TARGET]

- **Purpose:** Preserve a controlled change to studio structure, governance, architecture, shared systems, or authoritative records.
- **Owner:** VSOS owns change records for studio-level controlled changes.
- **Lifecycle:** Proposed -> Designed -> Approved, Rejected, Implemented, Superseded, or Archived.
- **Relationships:** Depends on audit findings, decision records, authority records, architecture records, risk records, and affected information objects.

### 4.19 Architecture Record [TARGET]

- **Purpose:** Preserve authoritative architecture definitions, boundaries, capabilities, information objects, operating-model definitions, controls, and interfaces.
- **Owner:** VSOS owns all studio-level architecture records.
- **Lifecycle:** Draft -> Approved, Superseded, Deprecated, or Archived.
- **Relationships:** Includes this architecture document set. Relates to decision records, change records, boundary decisions, capability definitions, and known unknowns.

### 4.20 Boundary Decision [TARGET]

- **Purpose:** Preserve a decision about whether a concern belongs inside or outside VSOS, and whether it belongs at studio level or product level.
- **Owner:** VSOS owns boundary decisions at the studio architecture level.
- **Lifecycle:** Proposed -> Decided -> Active, Revisited, Superseded, or Archived.
- **Relationships:** Depends on `SYSTEM_CONTEXT.md`, decision records, architecture records, source-of-truth determinations, and change records.

### 4.21 Source-of-Truth Determination [TARGET]

- **Purpose:** Preserve the single authoritative home for a fact or information object within an already-determined side or domain.
- **Owner:** VSOS owns source-of-truth determinations for studio-level information.
- **Lifecycle:** Proposed -> Decided -> Active, Superseded, or Archived.
- **Relationships:** Depends on boundary decisions. Relates to authoritative records, copies, derivatives, conflict records, and change records.

### 4.22 Known Unknown [TARGET]

- **Purpose:** Preserve an explicitly unresolved architectural or operating question without converting it into an assumption.
- **Owner:** VSOS owns studio-level known unknowns.
- **Lifecycle:** Recorded -> Active -> Resolved, Superseded, or Archived.
- **Relationships:** May arise from audits, architecture work, capability mapping, evidence gaps, source-of-truth conflicts, or boundary questions.

### 4.23 Audit Finding [TARGET]

- **Purpose:** Preserve what has been inspected, what was found, what remains unknown, and what should be preserved before change.
- **Owner:** VSOS owns studio-level audit findings.
- **Lifecycle:** Draft -> Accepted -> Reconciled, Superseded, or Archived.
- **Relationships:** May produce known unknowns, preservation needs, change records, source-of-truth determinations, and architecture conflicts.

### 4.24 Copy or Derivative [TARGET]

- **Purpose:** Identify information that is copied, summarized, transformed, or derived from an authoritative source without becoming authoritative itself.
- **Owner:** The authoritative owner remains the source object. VSOS owns copy or derivative labels for studio-level information.
- **Lifecycle:** Created -> Active -> Refreshed, Superseded, Deprecated, or Archived.
- **Relationships:** Must cite its source. May expose drift, duplication, or source-of-truth defects if it diverges from the authoritative record.

## 5. Knowledge Flow

Knowledge flow describes how information relates and compounds. It does not define workflow, sequence, roles, tools, or implementation.

At target architecture level, knowledge moves through VSOS in five patterns:

### 5.1 From Signal to Structured Information [TARGET]

Raw ideas, observations, market signals, and problem claims become usable only when they are captured as structured information objects such as ideas, problem statements, assumptions, hypotheses, or evidence.

The architectural requirement is that the information becomes classifiable, traceable, and owned. This document does not define how that capture occurs.

### 5.2 From Claim to Evidence [TARGET]

Claims become more useful when their truth status is explicit. Facts, assumptions, hypotheses, and recommendations must remain distinguishable.

Evidence may support, weaken, or refute a claim. The existence of a claim does not make it true; the existence of an experiment does not make it validated; the existence of a product does not prove demand.

### 5.3 From Evidence to Decision [TARGET]

Evidence, assumptions, hypotheses, risks, and alternatives inform decision records. Decision records preserve the judgment made, the basis for that judgment, and the conditions under which it should be revisited.

This is knowledge movement, not decision procedure. The control mechanics belong to `DECISION_CONTROL_ARCHITECTURE.md`.

### 5.4 From Venture Outcome to Studio Knowledge [TARGET]

Venture outcomes produce knowledge assets, venture summaries, reusable artifact records, risk insights, and portfolio patterns.

Failed experiments, killed ventures, and invalidated hypotheses are valuable knowledge. They must be preserved where they improve future studio judgment.

### 5.5 From Current Use to Historical Traceability [TARGET]

Information objects may become superseded, deprecated, or archived without losing value. Historical records preserve why the studio believed something, why it changed its mind, and what future work should not repeat.

## 6. Ownership Rules

### 6.1 Studio-Level Ownership [TARGET]

VSOS authoritatively owns studio-level information, including:

- Governance records.
- Architecture records.
- Capability definitions.
- Information-object definitions.
- Portfolio records.
- Lifecycle gate records.
- Studio-level decision records.
- Authority records for studio-level controlled decisions.
- Cross-product knowledge assets.
- Venture summaries and knowledge deposits.
- Source-of-truth determinations for studio-level information.
- Known unknowns and audit findings about studio-level concerns.

### 6.2 Product-Level Ownership [TARGET]

Product-internal information is outside VSOS. This includes product code, product-internal decisions, product-specific operational records, product-specific implementation details, and product-owned source-of-truth records.

VSOS may own studio-level records about a product, but it does not become the authoritative owner of the product's internal implementation.

### 6.3 Boundary Before Source of Truth [TARGET]

Boundary and ownership questions are resolved before source-of-truth determinations.

First, VSOS determines whether a concern belongs inside or outside VSOS, and whether it belongs at studio level or product level. Then, within the determined side or domain, the single authoritative home is identified.

### 6.4 Copies and Derivatives [TARGET]

Copies and derivatives are not authoritative unless explicitly designated as authoritative through change control.

Every copy or derivative must preserve a relationship to its source. If a copy conflicts with its source, the conflict is a defect until resolved.

### 6.5 Supersession and Deprecation [TARGET]

When information changes, the prior authoritative record is not silently overwritten as if it never existed. It is superseded, deprecated, or archived according to its lifecycle state.

This preserves decision memory and allows future readers to understand why the studio changed direction.

### 6.6 Unknowns [TARGET]

Unknown information must remain marked **[UNKNOWN]** until audit establishes its state.

An unknown may become a fact, assumption, hypothesis, recommendation, or discarded concern only after reconciliation. It must not be converted into current-state architecture by implication.

## 7. Scope Boundaries

### 7.1 What Belongs in This Document

This document owns:

- Durable information-object definitions.
- Authoritative ownership rules for information.
- Information lifecycle concepts.
- Knowledge-flow patterns.
- Copy, derivative, supersession, and archival principles.
- Information-level known unknowns.

### 7.2 What Belongs in `CAPABILITY_DOMAIN_MAP.md`

`CAPABILITY_DOMAIN_MAP.md` owns:

- Capability domains.
- Capability names.
- Capability purposes.
- Capability inputs, outputs, and dependencies.
- Architecture-level relationships among capabilities.

This document describes the information objects capabilities produce, consume, preserve, or govern. It does not redefine the capabilities.

### 7.3 What Belongs in `HUMAN_AGENT_OPERATING_MODEL.md`

`HUMAN_AGENT_OPERATING_MODEL.md` owns:

- Human role definitions.
- Agent role definitions.
- Allocation of work across roles.
- Participation in review and approval.
- Limits on delegated authority.

This document does not assign information objects to human roles, agent roles, or specific actors.

### 7.4 What Belongs in `DECISION_CONTROL_ARCHITECTURE.md`

`DECISION_CONTROL_ARCHITECTURE.md` owns:

- Authority paths.
- Lifecycle gates in motion.
- Change-control movement.
- Approval structures.
- Control records and escalation rules.

This document defines decision, authority, lifecycle, and change records as information objects, but it does not define how control operates.

### 7.5 What Belongs in `SYSTEM_CONTEXT.md`

`SYSTEM_CONTEXT.md` owns:

- The VSOS boundary.
- What is inside and outside VSOS.
- Actor categories at the boundary.
- External touchpoints.
- Studio-level versus product-level ownership at the context level.

This document depends on that boundary and does not redefine it.

### 7.6 What Belongs in Implementation

Implementation owns storage formats, file layouts, databases, applications, APIs, tools, vendors, automation, templates, prompts, and product-specific details.

Implementation must preserve the ownership, lifecycle, and traceability rules defined here, but those implementation choices are not part of this document.

## 8. Known Unknowns

The following architectural unknowns require future audit:

- Whether current studio records already map to the information objects defined here.
- Whether existing information has a single authoritative home.
- Whether existing records distinguish facts, assumptions, hypotheses, and recommendations.
- Whether existing decision records contain the rationale, evidence, alternatives, and revisit conditions required by the Constitution.
- Whether current portfolio records exist and whether they are studio-level, product-level, or duplicated.
- Whether existing knowledge assets have been preserved before replacement.
- Whether reusable artifacts exist and whether their studio-level records are distinct from their implementations.
- Whether existing product-level information has been copied into VSOS without clear ownership.
- Whether there are conflicts between existing documents, copies, derivatives, and authoritative records.
- Whether current lifecycle, authority, audit, and change records exist in sufficient form to support later control architecture.
- Whether existing unknowns have been mislabeled as facts or assumptions.
- Whether deprecated or superseded information is being retained for traceability.

These are unknowns, not assumptions. They remain **[UNKNOWN]** until audited and reconciled through the architecture governance and change-control process.

---

*Draft v0.1. Realizes the VSOS information & knowledge view. Subordinate to the Constitution and governed by `ARCHITECTURE_OVERVIEW.md`. All information objects and ownership rules are target architecture until audited; existing unaudited work remains unknown.*
