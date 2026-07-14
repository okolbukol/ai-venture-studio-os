# Review Package

## Repository Context

The document under review is:

- docs/standards/ADR_STANDARD.md

The authoritative inputs are:

- docs/constitution/CONSTITUTION.md
- docs/architecture/ARCHITECTURE_OVERVIEW.md
- docs/architecture/SYSTEM_CONTEXT.md
- docs/architecture/CAPABILITY_DOMAIN_MAP.md
- docs/architecture/INFORMATION_KNOWLEDGE_ARCHITECTURE.md
- docs/architecture/HUMAN_AGENT_OPERATING_MODEL.md
- docs/architecture/DECISION_CONTROL_ARCHITECTURE.md
- docs/architecture/INTEGRATION_INTERFACE_ARCHITECTURE.md
- docs/standards/DOCUMENTATION_STANDARD.md

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

## Information & Knowledge Architecture

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

Information objects have lifecycles. A lifecycle describes architectural state, not workflow sequence, and object-specific lifecycle states specialize these generic architectural lifecycle states.

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

Recommendations are preserved inside Decision Records and evidence-classification outputs; they are not authoritative standalone objects.

This rule applies to information objects as much as to prose. An unverified record is not made true by being recorded.

## 4. Information Objects

The following information objects are the durable studio-level objects VSOS must govern. All objects in this section are **[TARGET]**.

### 4.1 Idea [TARGET]

- **Purpose:** Capture a potential venture, problem, market signal, or strategic possibility before it is treated as validated.
- **Owner:** VSOS owns studio-level idea records. Product-internal idea details remain outside VSOS unless they are deposited through a studio-level interface.
- **Lifecycle:** Proposed -> Framed -> Advanced, Parked, Superseded, or Archived.
- **Relationships:** May produce assumptions, hypotheses, problem statements, opportunity records, or decision records. May draw on knowledge assets or Venture Thesis Records.

### 4.2 Problem Statement [TARGET]

- **Purpose:** Define the problem believed to exist, the affected customer or market context, and the evidence or uncertainty supporting that belief.
- **Owner:** VSOS owns studio-level problem statements used for venture assessment.
- **Lifecycle:** Draft -> Active -> Validated, Invalidated, Superseded, or Archived.
- **Relationships:** May originate from ideas. May support opportunity records, hypotheses, experiments, evidence, and validation assessments.

### 4.3 Opportunity Record [TARGET]

- **Purpose:** Represent a qualified studio-level opportunity that may justify venture concept definition or further validation.
- **Owner:** VSOS owns opportunity records at studio level.
- **Lifecycle:** Proposed -> Qualified -> Advanced, Rejected, Superseded, or Archived.
- **Relationships:** Depends on problem statements, evidence, assumptions, hypotheses, and Venture Thesis Records. May lead to venture concept records or decision records.

### 4.4 Venture Concept Record [TARGET]

- **Purpose:** Define a potential venture in terms of customer, problem, proposed value, key assumptions, and validation questions.
- **Owner:** VSOS owns Venture Concept Records for traceability and knowledge compounding. Only product-internal implementation moves outside the VSOS boundary.
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

### 4.25 Venture Thesis Record [TARGET]

- **Purpose:** Preserve the studio-level thesis that guides what kinds of ventures the studio should pursue and why.
- **Owner:** VSOS owns Venture Thesis Records as studio-level strategic information.
- **Lifecycle:** Draft -> Active -> Revised, Superseded, or Archived.
- **Relationships:** Informs ideas, opportunity records, venture concept records, validation assessments, portfolio records, decision records, risk records, and knowledge assets.

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

## Human-Agent Operating Model

# VSOS Human-Agent Operating Model

**Status:** Draft v0.1
**Type:** Architecture - foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **operating-model view**.

## Preamble

This document defines the operating-model view of the Venture Studio Operating System (VSOS): how work is allocated between durable human role categories and durable AI agent role categories across the studio.

It answers only one question:

**How is work allocated between human roles and AI agent roles across the Venture Studio?**

It does not define named people, staffing plans, organization charts, workflows, prompts, software, tools, vendors, models, APIs, code, products, or agent implementations.

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, the operating model in this document is **[TARGET]** unless explicitly marked otherwise. A **[TARGET]** role category or allocation rule is intended studio-level structure, not a verified current-state claim.

Any statement about existing people, existing agents, existing staffing, existing authority assignments, existing practices, or existing operating reality remains **[UNKNOWN]** until audited. This document does not assert that any current role category is already staffed or operational.

## 2. Purpose

VSOS separates human and AI agent responsibilities because the studio needs both leverage and accountability.

Humans retain judgment, authority, accountability, and approval. AI agents expand the studio's capacity to read, draft, analyze, compare, preserve, and prepare work. The separation protects the studio from confusing output with authority, speed with judgment, or automation with governance.

This operating model exists to:

- Preserve human authority over real-world actions and controlled changes.
- Define durable role categories without naming individuals or implementations.
- Make AI assistance useful without making it autonomous governance.
- Keep capabilities independent from whoever performs supporting work.
- Reduce dependency on any specific person, agent, model, or tool.
- Ensure outputs can be reviewed, approved, preserved, and traced.

## 3. Operating Principles

### 3.1 Human Authority Is Never Delegated

Human authority is not delegated to AI agents.

AI agents may prepare, draft, analyze, summarize, compare, classify, and recommend. They may not approve, authorize, or execute real-world actions that the Constitution reserves to humans.

### 3.2 AI Performs Work, Not Governance

AI agents contribute operating capacity. They do not own governance.

An agent output may inform a decision, but it is not a decision. An agent recommendation may support review, but it is not approval. An agent draft may become an authoritative record only after the required human and governance conditions are satisfied.

### 3.3 Capabilities Are Independent of Performers

Capabilities remain primary. Roles are secondary.

The capability architecture defines what the studio must be able to do. This operating model defines role categories that may participate in those capabilities. Changing who performs work does not change the capability itself.

### 3.4 Responsibilities Must Be Clearly Owned

Human and agent responsibilities must be distinct enough that review, approval, preservation, and accountability remain clear.

Shared participation is allowed. Ambiguous authority is not.

### 3.5 Automation Follows Understanding

No work is automated merely because it can be automated.

A capability must be understood, bounded, and reconciled with audited reality before automation is treated as appropriate. This document defines allocation principles only; automation design belongs outside this document.

### 3.6 Human Override Always Exists

A human with the relevant authority may reject, revise, pause, or supersede AI-prepared work.

Human override does not make unaudited facts true and does not bypass change control. It means accountability remains human.

### 3.7 No Dependency on Specific Individuals or AI Models

The operating model is described through durable role categories, not named individuals, specific agents, specific models, or implementation choices.

If the operating model works only because a particular person or particular model is present, that dependency is an architectural defect.

### 3.8 Truth Labels Apply to All Participants

Humans and agents must preserve the distinction between fact, assumption, hypothesis, and recommendation.

No participant may present assumption as fact, recommendation as approval, output as validation, or unknown current state as audited reality.

## 4. Human Roles [TARGET]

Human roles are durable role categories. They are not named people, job titles, staffing requirements, or an organization chart.

### 4.1 Founder [TARGET]

- **Purpose:** Provide ultimate studio-level intent, accountability, and judgment where foundational direction is required.
- **Responsibilities:** Set or clarify studio purpose, resolve unresolved strategic ambiguity, sponsor architecture and governance work, ensure the studio remains aligned with its mission.
- **Authority:** May hold final human authority where governance assigns it. May approve controlled decisions within assigned authority. Does not bypass the Constitution or change control.
- **Constraints:** Must not turn personal judgment into unrecorded governance. Must preserve decision records, evidence discipline, and the no-personal-dependency principle.

### 4.2 Executive Governance [TARGET]

- **Purpose:** Exercise human governance over consequential studio decisions, controlled changes, lifecycle gates, and external commitments.
- **Responsibilities:** Review decision context, assess evidence and risks, approve or reject controlled actions, preserve accountability for governance outcomes.
- **Authority:** May approve or reject actions within assigned governance scope. Holds authority only where explicitly assigned by governance.
- **Constraints:** Cannot delegate approval to AI agents. Cannot silently alter the Constitution, architecture, or controlled records. Must operate through change control where required.

### 4.3 Domain Expert [TARGET]

- **Purpose:** Provide specialized judgment in a domain relevant to a venture, risk, architecture decision, or evidence assessment.
- **Responsibilities:** Interpret domain evidence, identify domain-specific risks, challenge assumptions, advise on validity and constraints.
- **Authority:** May provide expert judgment and recommendations. Does not hold approval authority unless separately assigned by governance.
- **Constraints:** Must distinguish expertise from authority. Must label uncertainty and avoid converting opinion into fact.

### 4.4 Reviewer [TARGET]

- **Purpose:** Evaluate prepared work for correctness, completeness, consistency, evidence quality, and architectural fit.
- **Responsibilities:** Review drafts, identify gaps, test claims against authoritative sources, surface conflicts, recommend acceptance or revision.
- **Authority:** May accept work for further consideration within assigned review scope. Does not authorize real-world actions unless separately assigned by governance.
- **Constraints:** Must not treat review as final approval where approval is constitutionally required. Must preserve unresolved issues as unknowns or defects.

### 4.5 Operator [TARGET]

- **Purpose:** Carry out approved studio work within defined constraints and preserve the records produced by that work.
- **Responsibilities:** Execute authorized activities, maintain operating context, preserve outputs, route issues to the correct governance or review category.
- **Authority:** May act within explicitly approved scope. Does not create its own approval authority.
- **Constraints:** Must not proceed when authority, evidence, ownership, or boundary status is unclear. Must escalate uncertainty rather than assume permission.

### 4.6 Knowledge Steward [TARGET]

- **Purpose:** Protect the studio's authoritative knowledge, records, and source-of-truth discipline.
- **Responsibilities:** Maintain record quality, identify duplication, preserve lessons, support knowledge compounding, surface source-of-truth conflicts.
- **Authority:** May recommend preservation, deprecation, supersession, or reconciliation actions. Requires governance authority for controlled changes.
- **Constraints:** Must not silently overwrite or discard records. Must preserve traceability and state labels.

### 4.7 Architecture Steward [TARGET]

- **Purpose:** Protect coherence across the architecture document set and its relationship to the Constitution.
- **Responsibilities:** Review architecture consistency, identify overlap between views, preserve scope boundaries, surface architecture conflicts.
- **Authority:** May recommend architecture changes and identify defects. Requires authorized approval for changes to controlled architecture.
- **Constraints:** Must not move implementation detail into architecture. Must not resolve conflicts by silent edit.

## 5. AI Agent Roles [TARGET]

AI agent roles are durable architectural role categories. They are not specific agents, prompts, models, software, tools, or implementations.

All AI agent roles share the same authority limit: they may prepare work for human review, but they do not approve, authorize, own governance, or execute real-world actions reserved to humans.

### 5.1 Research Agent [TARGET]

- **Purpose:** Prepare research material that helps humans and other roles understand problems, markets, customers, evidence, constraints, and unknowns.
- **Responsibilities:** Gather and summarize relevant information, distinguish fact from assumption, identify evidence gaps, surface unknowns.
- **Authority Limits:** Cannot treat research output as validation. Cannot contact real people, publish, spend, or make commitments without human approval.
- **Inputs:** Research questions, venture thesis records, problem statements, hypotheses, evidence needs, known unknowns.
- **Outputs:** Research summaries, evidence candidates, uncertainty lists, source notes, recommendation drafts.

### 5.2 Analysis Agent [TARGET]

- **Purpose:** Prepare structured analysis of evidence, decisions, risks, trade-offs, and alternatives.
- **Responsibilities:** Compare options, classify evidence, test consistency, identify risks, prepare recommendation drafts.
- **Authority Limits:** Cannot decide, approve, or make governance judgments final. Cannot present analysis as external validation.
- **Inputs:** Evidence records, assumptions, hypotheses, decision questions, portfolio records, risk records.
- **Outputs:** Analysis summaries, comparison notes, risk observations, decision-support drafts, unresolved questions.

### 5.3 Repository Engineer [TARGET]

- **Purpose:** Prepare and maintain repository-contained artifacts under human instruction and governance constraints while preserving repository integrity.
- **Responsibilities:** Prepare repository-contained artifacts, apply approved repository updates, preserve structural consistency, verify changed artifacts, report what changed.
- **Authority Limits:** Cannot approve its own changes, alter governance outside approved scope, or delete protected work without explicit human approval.
- **Inputs:** Approved task instructions, authoritative documents, review comments, repository-scoped change requirements, validation requirements.
- **Outputs:** Prepared artifacts, applied updates, validation reports, change summaries, conflict reports.

### 5.4 Validation Agent [TARGET]

- **Purpose:** Prepare validation support by organizing hypotheses, evidence, assumptions, and confidence questions.
- **Responsibilities:** Identify testable claims, summarize evidence strength, flag vanity metrics, distinguish validation from deployment.
- **Authority Limits:** Cannot declare a venture validated as a final decision. Cannot treat its own output as customer evidence.
- **Inputs:** Venture concept records, hypotheses, evidence records, experiment records, validation criteria, risk records.
- **Outputs:** Validation-support summaries, evidence-strength notes, invalidation concerns, recommendation drafts, unknowns.

### 5.5 Documentation Agent [TARGET]

- **Purpose:** Prepare content and documentation changes that are readable, consistent, traceable, and aligned with authoritative sources.
- **Responsibilities:** Author documentation content, improve documentation quality, maintain documentation consistency, summarize existing records, identify duplication, preserve citations to authoritative sources, flag scope drift.
- **Authority Limits:** Cannot make documents authoritative without the required review and approval. Cannot silently replace or deprecate existing records.
- **Inputs:** Authoritative records, architecture documents, knowledge assets, decision records, review comments.
- **Outputs:** Draft documents, summaries, consistency notes, deprecation candidates, documentation-gap reports.

### 5.6 Knowledge Stewardship Agent [TARGET]

- **Purpose:** Prepare support for preserving, classifying, and connecting studio knowledge.
- **Responsibilities:** Identify knowledge assets, map relationships between records, flag source-of-truth conflicts, prepare preservation candidates.
- **Authority Limits:** Cannot designate a new authoritative source by itself. Cannot archive, delete, or supersede records without required approval.
- **Inputs:** Knowledge assets, venture summaries, reusable artifact records, source-of-truth determinations, audit findings.
- **Outputs:** Knowledge maps, preservation notes, duplicate-record flags, source-of-truth issue reports, draft knowledge deposits.

### 5.7 Review Support Agent [TARGET]

- **Purpose:** Prepare review support for humans by checking artifacts against governing sources and stated requirements.
- **Responsibilities:** Compare drafts against authoritative documents, identify missing sections, check state labels, surface conflicts.
- **Authority Limits:** Cannot approve artifacts. Cannot certify compliance as final governance approval.
- **Inputs:** Draft artifacts, authoritative inputs, review criteria, architecture principles, known constraints.
- **Outputs:** Review notes, issue lists, consistency checks, suggested corrections, unresolved conflicts.

## 6. Allocation Principles

### 6.1 Capabilities Remain Primary

Capabilities define what the studio must be able to do. Roles define who or what may participate in supporting those capabilities.

No role owns a capability merely by participating in it.

### 6.2 Roles Are Secondary

Human and agent role categories are assigned around the needs of a capability, decision, record, or review.

Changing role participation does not change the capability definition, information object definition, system boundary, or control requirement.

### 6.3 Multiple Roles May Participate

The same capability may involve multiple human roles and multiple AI agent roles.

Participation does not imply authority. Authority follows the Constitution and the later decision-control architecture.

### 6.4 Allocation Follows Risk and Authority

Work with real-world consequences, governance consequences, legal or financial exposure, reputation risk, deletion risk, or external commitment requires human authority.

AI agents may prepare, analyze, summarize, and preserve supporting material, but authority remains human.

### 6.5 Allocation Follows Evidence Quality

Where evidence is weak, uncertain, or disputed, humans retain judgment and review. AI agents may help expose the uncertainty, but they cannot resolve uncertainty by assertion.

### 6.6 Allocation Follows Preservation Needs

When work produces reusable knowledge, decision rationale, evidence, or architecture implications, roles must preserve the relevant information objects defined by `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`.

## 7. Collaboration Rules

### 7.1 Agents Prepare; Humans Review

AI agents may prepare drafts, analyses, summaries, comparisons, and recommendations. Humans review the outputs and decide whether they are accepted, revised, rejected, or escalated.

### 7.2 Humans Approve; Agents Do Not

Approval remains human. Agent output cannot substitute for approval, even when the output is accurate, useful, or requested.

### 7.3 Agents Preserve Information

AI agents may help preserve records, classify information, identify relationships, and draft knowledge deposits. Preservation support does not make the agent the owner of the knowledge or the authority over the record.

### 7.4 Humans Own Accountability

Humans remain accountable for decisions, approvals, and external effects. AI participation does not reduce human accountability.

### 7.5 Uncertainty Is Escalated

When authority, evidence, ownership, boundary status, or source of truth is unclear, the uncertainty is preserved and surfaced rather than silently resolved.

### 7.6 Conflicts Route to Governance

If human judgment, agent output, authoritative documents, or existing records conflict, the conflict is recorded and resolved through the appropriate governance and change-control structures.

### 7.7 No Silent Replacement

No participant silently overwrites, deletes, or supersedes existing work. Preservation before replacement applies to both human and AI-assisted work.

## 8. Scope Boundaries

### 8.1 What Belongs in This Document

This document owns:

- Durable human role categories.
- Durable AI agent role categories.
- Responsibility allocation principles.
- Collaboration rules between human and AI agent roles.
- Operating-model known unknowns.

### 8.2 What Belongs in `CAPABILITY_DOMAIN_MAP.md`

`CAPABILITY_DOMAIN_MAP.md` owns:

- Capability domains.
- Capability names.
- Capability purposes.
- Capability inputs, outputs, and dependencies.
- Capability relationships.

This document allocates role participation around capabilities; it does not redefine capabilities or move capability ownership into roles.

### 8.3 What Belongs in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`

`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` owns:

- Information objects.
- Authoritative homes for records.
- Information lifecycle concepts.
- Knowledge-flow patterns.
- Source-of-truth and ownership rules for information.

This document identifies which role categories may help prepare, review, or preserve information; it does not redefine the information architecture.

### 8.4 What Belongs in `DECISION_CONTROL_ARCHITECTURE.md`

`DECISION_CONTROL_ARCHITECTURE.md` owns:

- Authority paths.
- Lifecycle gates in motion.
- Approval structures.
- Control records.
- Escalation and change-control structures.

This document states that human authority is required; it does not define detailed control paths.

### 8.5 What Belongs in `INTEGRATION_INTERFACE_ARCHITECTURE.md`

`INTEGRATION_INTERFACE_ARCHITECTURE.md` owns:

- Interfaces between capabilities.
- Interfaces between VSOS and product repositories.
- Interfaces between VSOS and the outside world.
- Exchange points and integration rules.

This document defines role categories that may participate around interfaces; it does not define the interfaces.

### 8.6 What Belongs in Implementation

Implementation owns specific people, staffing plans, prompts, models, tools, software, APIs, automations, product-specific assignments, and execution detail.

Implementation must conform to this operating model but is not defined here.

## 9. Known Unknowns

The following architectural unknowns require future audit:

- Which human role categories currently exist in practice.
- Which AI agent role categories currently exist in practice.
- Who currently holds human approval authority for each controlled decision category.
- Whether existing agents have defined scopes, inputs, outputs, and owners.
- Whether any current agent is operating outside constitutional authority limits.
- Whether current work depends on named individuals in a way that violates the no-personal-dependency principle.
- Whether current human and agent responsibilities are ambiguous, duplicated, or conflicting.
- Whether current practices preserve fact, assumption, hypothesis, and recommendation labels.
- Whether current review and approval practices distinguish agent preparation from human approval.
- Whether existing knowledge deposits preserve the information objects required by the information architecture.
- Whether current role allocation creates gaps in capability support.
- Whether current architecture or governance documents assign capability ownership to roles in conflict with the capability view.

These are unknowns, not assumptions. They remain **[UNKNOWN]** until audited and reconciled through the architecture governance and change-control process.

---

*Draft v0.1. Realizes the VSOS operating-model view. Subordinate to the Constitution and governed by `ARCHITECTURE_OVERVIEW.md`. All role categories and allocation rules are target architecture until audited; existing unaudited work remains unknown.*

## Decision and Control Architecture

# VSOS Decision and Control Architecture

**Status:** Draft v0.1
**Type:** Architecture — foundational
**Precedence:** Subordinate to the Constitution. Governed by `ARCHITECTURE_OVERVIEW.md`. Realizes the **control view**.

## Preamble

This document defines the control view of the Venture Studio Operating System (VSOS): how authority, governance, approval, escalation, and change control flow through the studio.

It answers only one question:

**How does authority, governance, approval, escalation, and change control flow through VSOS?**

It puts the governance capabilities named in `CAPABILITY_DOMAIN_MAP.md` into motion, but does not redefine them. It relies on the governance records defined in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`, but does not redefine those objects. It assigns authority categories to the role categories defined in `HUMAN_AGENT_OPERATING_MODEL.md`, but does not redefine those roles. It does not define workflows, staffing, tools, interfaces, or product-internal governance.

---

## 1. State Conventions

Because the studio's existing work has not yet been audited, every authority, gate, and control rule in this document is **[TARGET]** unless explicitly marked otherwise. A **[TARGET]** control structure is intended studio-level architecture, not a verified current-state claim.

Any statement about who currently holds authority, which gates currently operate, or how decisions are currently made remains **[UNKNOWN]** until audited. This document does not assert that any current authority holder, gate, or control record already exists.

## 2. Purpose

Control is architectural. A studio's operating system is defined as much by how authority and change flow through it as by what it can do.

This document exists to:

- Define the durable categories of decision authority the studio requires, without naming individuals.
- Define the architectural gates at which a transition or action is authorized or blocked.
- State which governance records must exist for a decision to be in force.
- Define how uncertainty and conflict escalate.
- Preserve human authority over every real-world action and controlled change (Constitution §6, §7).

It translates the Constitution's authority rules (§6), decision discipline (§8), lifecycle gating (§5), preservation rule (§9), and change-control process (§13) into a stable control structure that every capability, record, and role passes through.

## 3. Decision Principles

These principles constrain all authority, gates, and escalation defined below. Each traces to the Constitution.

1. **Human authority.** Every real-world action touching people, money, reputation, or law, and every controlled change, is authorized by a human. Agents prepare; humans decide. *(Constitution §6, §7)*
2. **Authority is never held by an AI agent.** No authority category in this document may be held, exercised, or delegated to an AI agent. An agent may prepare the material a decision rests on; it may never make, approve, or execute the decision. *(§7; `HUMAN_AGENT_OPERATING_MODEL.md` §3.1)*
3. **Evidence before approval.** No gate is passed on assertion. The evidence a decision rests on must exist and be classified before authority is exercised. *(§4, §8)*
4. **Progressive validation.** Authority to progress scales with the strength of evidence. Strong pre-payment evidence may justify progression; payment is the strongest validation and is never assumed before it occurs. *(§4)*
5. **Separation of preparation and approval.** The party that prepares a decision is architecturally distinct from the authority that approves it. Preparation is not approval, however accurate or complete. *(§6; operating model §7.1–§7.2)*
6. **Escalation over assumption.** When authority, evidence, ownership, or boundary status is unclear, the matter escalates to the authority with jurisdiction. Uncertainty is surfaced, never resolved by assumption. *(operating model §7.5)*
7. **Auditability.** Every consequential decision leaves a governance record sufficient for a later reader to understand what was decided, on what basis, by which authority, and when it should be revisited. *(§8)*
8. **Preservation before replacement.** No controlled record, decision, or structure is removed or superseded before it is inspected, understood, and its replacement justified and approved. *(§9)*
9. **Change control.** Every controlled change follows Audit → Design → Approval → Implementation. Silent change to governance or architecture is prohibited. *(§13)*

## 4. Decision Authorities [TARGET]

The following are durable **categories of authority** — kinds of decision rights the studio requires. They are not roles and not individuals. Governance assigns each category to one or more human role categories defined in `HUMAN_AGENT_OPERATING_MODEL.md`; **which role or person holds each category is [UNKNOWN] pending audit and governance assignment** (Constitution Open Questions). No category may be held by an AI agent (§3.2).

A single human may hold several categories, and a category may be shared, provided the separation-of-preparation-and-approval principle (§3.5) is preserved.

### 4.1 Constitutional Authority [TARGET]

- **Purpose:** Authorize amendments to the Constitution and resolve conflicts where the Constitution is unclear.
- **Authority:** Highest authority in the studio; approves constitutional amendments under the change-control process; interprets the Constitution where a conflict cannot be resolved at a lower authority.
- **Constraints:** Bound by the Constitution's own change-control process (§13); may not amend by silent edit or expedience; may not delegate to an agent.

### 4.2 Architecture Authority [TARGET]

- **Purpose:** Authorize changes to the architecture document set and resolve conflicts between architecture views.
- **Authority:** Approves changes that alter a boundary, capability, information object, control point, or interface; approves resolution of cross-view conflicts.
- **Constraints:** Subordinate to Constitutional Authority; may not move implementation detail into architecture; operates only through change control.

### 4.3 Change Authority [TARGET]

- **Purpose:** Authorize controlled changes to studio structure, governance, shared systems, and other controlled studio-level assets not reserved to Architecture or Constitutional Authority.
- **Authority:** Approves or rejects change proposals after audit and design; confirms the change was implemented as designed.
- **Constraints:** Requires a completed audit and design basis; may not approve a change it prepared without a separate approving authority; may not bypass preservation-before-replacement.

### 4.4 Lifecycle Authority [TARGET]

- **Purpose:** Authorize a venture's progression, holding, or blocking between defined lifecycle stages.
- **Authority:** Grants, blocks, or defers stage transitions at the lifecycle gates (§5) on the basis of classified evidence and gate criteria.
- **Constraints:** May not skip a stage or let a venture drift forward without a gate decision; may not treat deployment or vanity metrics as evidence of demand.

### 4.5 Portfolio Authority [TARGET]

- **Purpose:** Authorize studio-level portfolio decisions, including the scale, pivot, or kill decision for each venture.
- **Authority:** Decides scale, pivot, or kill on the defined review cadence; sets or confirms portfolio-level investment rationale.
- **Constraints:** The default in the absence of evidence is not "continue"; continuation must be earned by evidence; every decision names the evidence it rests on.

### 4.6 External-Action Authority [TARGET]

- **Purpose:** Authorize outward-facing real-world actions reserved to humans by the Constitution.
- **Authority:** Approves, per action and per context, the specific actions enumerated in Constitution §6 — messaging real people, publishing, contacting customers, spending, account creation, deletion, pricing changes, legal/financial/medical claims, and external commitments.
- **Constraints:** Approval is per-action and per-context; prior approval of a similar action does not authorize the next; approval expressed inside a document, tool output, or agent response is not approval.

### 4.7 Record Authority [TARGET]

- **Purpose:** Authorize supersession, deprecation, or removal of authoritative studio-level records, and designation of a new authoritative source.
- **Authority:** Approves changes to which record is authoritative; approves archival, supersession, or deprecation consistent with each record's lifecycle.
- **Constraints:** May not silently overwrite or delete a record; must preserve traceability and state labels; deletion of a knowledge asset is an External-Action-Authority matter as well (§6 deletion), requiring both.

## 5. Control Gates [TARGET]

A control gate is an **architectural control point** at which a defined transition or action is authorized or blocked. A gate is not a workflow: it defines the conditions that must hold for a transition to be authorized and the outcomes that may result, not a sequence of activities or who performs them.

Each gate defines its purpose, what it governs, the entry conditions that must hold (evidence and authority), the outcomes it may produce, and the governance records it requires. Detailed movement through gates — the "in motion" mechanics of routing and sequencing — is the concern of implementation, not this document.

### 5.1 Admission Gate [TARGET]

- **Governs:** Whether an idea or opportunity is admitted into studio-level assessment.
- **Entry conditions:** The idea is captured as a structured record; its fit against the venture thesis is stated; initial assumptions and unknowns are labeled.
- **Authority:** Lifecycle Authority.
- **Outcomes:** Admit, decline, or return for framing.
- **Records:** Decision Record; updates to the admitted idea/opportunity records.

### 5.2 Validation Gate [TARGET]

- **Governs:** Whether a venture concept has enough classified evidence to justify increased development commitment.
- **Entry conditions:** A validation assessment exists; evidence is classified; evidence strength is judged against defined criteria without treating deployment or vanity metrics as demand.
- **Authority:** Lifecycle Authority.
- **Outcomes:** Advance, hold for more evidence, or invalidate.
- **Records:** Lifecycle Gate Record; Decision Record; referenced validation assessment and evidence.

### 5.3 Build-Readiness Gate [TARGET]

- **Governs:** Whether a validated venture may commit to increased build investment.
- **Entry conditions:** Validation is cleared; readiness criteria are met; risks and constraints are recorded.
- **Authority:** Lifecycle Authority, with External-Action Authority for any spend or external commitment the commitment entails.
- **Outcomes:** Authorize development commitment, defer, or return to validation.
- **Records:** Lifecycle Gate Record; Decision Record; Authority Record for any reserved action.

### 5.4 Portfolio-Review Gate [TARGET]

- **Governs:** The recurring studio-level review of every venture against defined criteria.
- **Entry conditions:** Portfolio records are current; growth or validation evidence for the period is classified.
- **Authority:** Portfolio Authority.
- **Outcomes:** Confirm current state, flag for a scale/pivot/kill decision, or require more evidence.
- **Records:** Decision Record; updated portfolio records.

### 5.5 Scale / Pivot / Kill Gate [TARGET]

- **Governs:** The explicit studio-level decision to scale, pivot, or kill a venture.
- **Entry conditions:** A portfolio review has flagged the venture; the evidence and rationale for the decision are recorded; the default is not "continue."
- **Authority:** Portfolio Authority.
- **Outcomes:** Scale, pivot, or kill, each recorded with its evidence and next milestone or follow-on knowledge need.
- **Records:** Decision Record; updated portfolio record; knowledge-harvest need on pivot or kill.

### 5.6 Decommission-Review Gate [TARGET]

- **Governs:** Whether a killed or retired venture may be decommissioned, and on what terms knowledge is preserved first.
- **Entry conditions:** A kill or retirement decision exists; reusable knowledge and artifacts have been identified for preservation (preservation before replacement).
- **Authority:** Portfolio Authority, with External-Action Authority for any deletion, account closure, or external effect, and Record Authority for supersession of authoritative records.
- **Outcomes:** Authorize decommission with preservation, defer until preservation is complete, or block.
- **Records:** Decision Record; Authority Record; venture summary and knowledge deposits.

### 5.7 External-Action Authorization Gate [TARGET]

- **Governs:** Every outward-facing effect reserved to humans by Constitution §6, wherever it arises in the studio.
- **Entry conditions:** The specific action, its context, and its consequences are stated; the action is prepared but not executed.
- **Authority:** External-Action Authority.
- **Outcomes:** Authorize this action in this context, or decline.
- **Records:** Authority Record; Decision Record where consequential.
- **Note:** This gate is cross-cutting. No interface, capability, or agent may reach the outside world except through it (System Context §8).

### 5.8 Change-Control Gate [TARGET]

- **Governs:** Every controlled change to studio structure, governance, architecture, or shared systems (Constitution §13).
- **Entry conditions:** An audit of the current state exists; a design with trade-offs and alternatives exists; the reason preservation-and-evolution was insufficient is stated.
- **Authority:** Change Authority; Architecture Authority for architecture changes; Constitutional Authority for constitutional amendments.
- **Outcomes:** Approve, reject, or return for redesign; after implementation, verify against the design.
- **Records:** Change Record; Decision Record; Authority Record; Audit Finding.

## 6. Decision Records

The durable governance records are defined as information objects in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4. This document does not redefine them; it states their role in control.

From the control view, a decision is not in force until its required records exist. Specifically:

- **Decision Record** (`INFO` §4.10) — the authoritative record of a consequential decision: what was decided, by which authority, on what evidence and assumptions, and under what conditions it is revisited (Constitution §8). A decision without its record is not an authoritative decision.
- **Authority Record** (`INFO` §4.11) — evidence that a reserved action or controlled decision received the required human authorization. A §6 action without an Authority Record is unauthorized.
- **Lifecycle Gate Record** (`INFO` §4.12) — the documented gate decision permitting or blocking a stage transition. Progression without one is drift, which the architecture prohibits.
- **Change Record** (`INFO` §4.18) — the record of a controlled change across Audit → Design → Approval → Implementation.
- **Boundary Decision** (`INFO` §4.20) and **Source-of-Truth Determination** (`INFO` §4.21) — the records fixing what is inside VSOS and which source is authoritative, produced when a gate or escalation resolves an ownership question.
- **Risk Record** (`INFO` §4.17) and **Audit Finding** (`INFO` §4.23) — the recorded constraints and inspection results that gates and authorities rely on.

The control requirement is singular: **authority is exercised only against evidence, and its exercise leaves a record.** The record's format, storage, and location are implementation and are not defined here.

## 7. Escalation Principles

Escalation is the architectural response to uncertainty and conflict. It has no workflow here — only the conditions that trigger it and the direction it takes.

### 7.1 Escalation Triggers [TARGET]

A matter escalates when any of the following holds: the authority for a decision is unclear or absent; the evidence is insufficient, disputed, or unclassified; the boundary or ownership of the concern is ambiguous; two authoritative sources conflict; a human and an agent recommendation disagree in a way that affects a decision; or a proposed action falls outside the scope of any assigned authority.

### 7.2 Escalation Direction [TARGET]

A matter escalates to the authority category with jurisdiction over it: lifecycle matters to Lifecycle Authority, portfolio matters to Portfolio Authority, controlled changes to Change or Architecture Authority, reserved actions to External-Action Authority, record and source-of-truth matters to Record Authority, and unresolved conflicts of authority or constitutional interpretation to Constitutional Authority. Where jurisdiction itself is unclear, the matter escalates upward until an authority with clear jurisdiction is reached.

### 7.3 Escalation Constraints [TARGET]

Escalation never transfers authority to an AI agent. Escalation does not convert an unknown into a fact, and does not bypass change control. An escalated matter is preserved as a record (a Known Unknown, conflict record, or decision record as appropriate) so that its resolution — or its continued open state — is auditable.

## 8. Scope Boundaries

### 8.1 What Belongs in This Document

This document owns: durable decision-authority categories; architectural control gates; escalation principles; and the control-view statement of which records must exist for a decision to be in force.

### 8.2 What Belongs in `CAPABILITY_DOMAIN_MAP.md`

The capability map owns the governance capabilities (Human Authority Control, Lifecycle Gate Control, Change Control Stewardship, and others) as durable abilities. This document puts those abilities in motion as authorities and gates; it does not redefine the capabilities.

### 8.3 What Belongs in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`

The information architecture owns the definitions, ownership, and lifecycle of the governance records (Decision Record, Authority Record, Lifecycle Gate Record, Change Record, and others). This document references those records and states their role in control; it does not define them.

### 8.4 What Belongs in `HUMAN_AGENT_OPERATING_MODEL.md`

The operating model owns the human and AI role categories and how work is allocated between them. This document defines the authority categories that governance assigns to those roles; it does not define the roles, staffing, or assignment to individuals.

### 8.5 What Belongs in `INTEGRATION_INTERFACE_ARCHITECTURE.md`

The integration architecture owns the interfaces between capabilities, between VSOS and product repositories, and between VSOS and the outside world. This document defines the authorization that outward-facing interfaces must pass through (§5.7); it does not define the interfaces.

### 8.6 What Belongs in `SYSTEM_CONTEXT.md`

The context view owns the boundary and the actors. This document controls authority and change within that boundary; it does not redefine the boundary.

### 8.7 What Belongs in Implementation

Implementation owns the movement through gates, routing and sequencing, notification, record storage and format, tools, and any product-specific governance. This document defines the control architecture those implementations must conform to; it does not define them.

## 9. Known Unknowns

The following are explicitly unresolved and must be established by audit before this control view can be marked [CURRENT]. They are recorded as known unknowns, not assumptions:

- Who currently holds each authority category, and whether any category is currently held by an AI agent in violation of §3.2.
- Which control gates currently operate in practice, and whether ventures currently progress without gate decisions.
- Whether current decisions leave records sufficient for the auditability principle.
- Whether reserved §6 actions currently occur without an Authority Record.
- Whether current change to governance or architecture occurs outside change control.
- Whether preparation and approval are currently separated, or currently collapsed into one party.
- Whether current escalation preserves uncertainty as a record or resolves it silently.
- Where authority is currently ambiguous, duplicated, or unassigned across categories and roles.

Each of these feeds the audit that precedes any redesign (preservation before replacement, Constitution §9).

---

*Draft v0.1. Realizes the control view of the VSOS architecture. Subordinate to the Constitution; governed by `ARCHITECTURE_OVERVIEW.md`. Amendable only through change control. All authorities, gates, and control rules are target architecture until audited; current-state control remains unknown, and no authority is held by an AI agent.*

## Integration Interface Architecture

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

## Documentation Standard

# VSOS Documentation Standard

**Status:** Draft
**Version:** 0.1.0
**Type:** Standard — foundational
**Owner:** Architecture Steward [TARGET — pending governance assignment]
**Authority:** Architecture Authority [TARGET — pending governance assignment]
**Last Updated:** [UNKNOWN — set on ratification]
**Related Documents:** `CONSTITUTION.md`; the seven Core Architecture documents in `docs/architecture/`.

## Preamble

This document defines how every VSOS document must be written. It is a standard, not an architecture document: it governs the *form, metadata, versioning, and reference discipline* of documents, not the *content* of the architecture. Where it needs an architectural fact, it references the authoritative document rather than restating it.

If this standard conflicts with the Constitution or the Core Architecture, those win, and the conflict is resolved through change control (Constitution §13).

---

## 1. Purpose

A single, shared documentation standard exists so that every VSOS document is legible, traceable, and governable in the same way. It serves the Constitution's rules that documentation is written to be read (§11), that every fact has one authoritative home (§10), and that truth, targets, and unknowns stay distinct (§4).

Concretely, this standard makes each document state what it is, what state it is in, who owns it, what authority governs it, and how it relates to the rest of VSOS — so a later reader, human or agent, can trust and navigate it without external context.

## 2. Scope

This standard applies to every document authored inside VSOS, including:

- Governance documents (the Constitution and subordinate governance).
- Architecture documents.
- Standards (including this one).
- Architecture Decision Records (ADRs).
- Playbooks.
- Agent Specifications.
- Repository documentation.

It governs how those documents are written and maintained. It does not govern their subject matter: it does not define architecture, implementation, repository structure, workflows, agent behavior, or any tool or vendor. Those remain the concern of the documents and layers that own them.

## 3. Document Classification

Every VSOS document declares exactly one class. The class sets expectations for authority, versioning, and permanence.

- **Constitution** — the single ratified foundational governance document; supreme where conflicts arise.
- **Architecture** — a document realizing one architecture view; defines durable structure.
- **Standard** — a rule set governing how work or documents are produced (such as this document).
- **ADR (Architecture Decision Record)** — a record of one consequential decision, its context, alternatives, and consequences.
- **Playbook** — repeatable guidance for performing a kind of studio work.
- **Agent Specification** — the durable definition of an agent role's scope, inputs, outputs, limits, and owner.
- **Governance document** — a subordinate governance rule set not covered by the classes above.
- **Repository documentation** — orientation and navigation material for a repository or area.

A document that appears to span two classes is split, or its primary class is declared and the secondary concern is referenced, never merged.

## 4. Required Metadata

Every VSOS document opens with a metadata block containing at least:

- **Status** — one of the values defined in §6.
- **Version** — a semantic version per §5.
- **Type / Class** — the document class per §3.
- **Owner** — the role category (per `HUMAN_AGENT_OPERATING_MODEL.md`) accountable for the document. Never a named individual (Constitution §3.5).
- **Authority** — the authority category (per `DECISION_CONTROL_ARCHITECTURE.md` §4) whose approval governs changes to the document.
- **Last Updated** — the date of the most recent approved change; `[UNKNOWN]` until first ratification.
- **Related Documents** — the authoritative documents this one references or depends on.

Metadata states facts about the document, not about the studio's operating reality. Absent or placeholder metadata is itself a documentation defect.

## 5. Versioning Rules

VSOS documents use semantic versioning: **MAJOR.MINOR.PATCH**.

- **Pre-ratification** documents sit below `1.0.0` (for example `0.1`), signaling draft status.
- **Ratification** to the first stable, governed version is `1.0.0`.
- **MAJOR** increments when a change alters or removes a defined element the document owns — a principle, boundary, capability, information object, control point, interface, or standard rule.
- **MINOR** increments when a document adds a new such element without breaking existing ones.
- **PATCH** increments for wording, clarification, or formatting that does not change meaning.

Whether a change is MAJOR, MINOR, or PATCH is judged against what the document authoritatively owns. Wording-only edits that change no owned element do not require re-versioning of architecture, consistent with `ARCHITECTURE_OVERVIEW.md` §5. Every version change is recorded per §13 and approved by the document's stated Authority.

## 6. Status Definitions

A document carries exactly one status:

- **Draft** — under development; not authoritative. The default for any new document. A draft is never self-ratifying.
- **Approved** — reviewed and accepted by its stated Authority for use, but not elevated to ratified/foundational standing where that distinction applies.
- **Ratified** — formally established as authoritative and foundational through the change-control process; reserved for documents that carry that standing (such as the Constitution).
- **Deprecated** — no longer authoritative or recommended, retained for traceability; supersession is recorded.
- **Archived** — retained for historical reference only; not in active use.

Status changes are discrete, explicit acts by the document's Authority, never implied by editing. Draft is the starting state; movement to Approved or Ratified is a recorded decision (Constitution §8, §13).

## 7. Cross-Reference Rules

- A document references the single authoritative source for anything outside its own concern; it does not restate that source (Constitution §10; `ARCHITECTURE_OVERVIEW.md` §2, principle 4).
- References name the target document and, where useful, its section (for example, `DECISION_CONTROL_ARCHITECTURE.md` §5).
- A reference points to the authoritative document, not to a copy or derivative of it.
- When a referenced document is superseded, references to it are updated, deprecated, or repointed through change control; dangling references are defects.
- A document does not reference implementation, tools, or vendors to establish an architectural or governance fact.

## 8. Terminology Rules

- Terms defined by the Constitution or Core Architecture are used with their defined meaning and are not redefined. Where a term's authoritative definition matters, the document references its home rather than restating it.
- A document does not introduce a new term for a concept that already has an authoritative name; reuse over reinvention (Constitution §3.9).
- A document introducing a genuinely new term states its meaning once, clearly, and thereafter uses it consistently.
- The four truth categories — fact, assumption, hypothesis, recommendation — are used with the meanings fixed by Constitution §4 and are kept distinct.

## 9. Markdown Style Rules

- Documents are written in Markdown, structured with a single top-level title and hierarchical section headings.
- A document opens with the metadata block (§4) and a short preamble stating what the document is and what single question or purpose it serves.
- Prose is preferred for reasoning; lists are used for enumerable items, not as a substitute for explanation.
- Length is a cost (Constitution §3.10, §11): documents stay as short as their purpose allows, and detail belonging to a lower layer is referenced, not absorbed.
- Formatting choices (exact heading depth, list style) are conventions, not architecture; this section sets expectations, not a rigid template, and remains technology-neutral.

## 10. Naming Rules

- Document filenames are descriptive, stable, and consistent within their class and directory.
- A document's title matches its purpose and its filename's intent.
- Names describe the document's concern, not a tool, vendor, person, or implementation.
- Renaming an authoritative document is a change-controlled action, because references depend on the name.

## 11. Reference and Citation Rules

- A claim that rests on another document cites that document as its source.
- A copied or derived passage is labeled as a copy or derivative and cites its authoritative source (Constitution §10; `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4.24, §6.4); it is not presented as authoritative.
- External or evidentiary claims are attributed to their source; unverified claims are labeled per §12 rather than asserted.
- A document does not fabricate a citation or attribute a claim to a source that does not support it (Constitution §4).

## 12. Unknowns

Every VSOS document uses the three state labels consistently with the Core Architecture:

- **[CURRENT]** — reconciled with audited reality; verified true today.
- **[TARGET]** — intended structure, defined but not yet reconciled with reality.
- **[UNKNOWN]** — existence or details not yet established; pending audit.

Rules of use:

- Unaudited claims about existing systems, products, or practice remain **[UNKNOWN]**; they are never presented as **[CURRENT]** by implication.
- Intended structure is **[TARGET]** until an audit reconciles it; reconciliation happens through the change process, not silent edits.
- A document does not convert an **[UNKNOWN]** into a fact, assumption, or **[CURRENT]** claim without recorded reconciliation.
- Where a label is omitted, the document states its default, as the Core Architecture documents do.

## 13. Change History Rules

- Every approved change to a document is recorded: what changed, the resulting version, the approving Authority, and the date.
- Changes follow Audit → Design → Approval → Implementation (Constitution §13); silent edits to governed documents are prohibited.
- Prior authoritative versions are Deprecated or Archived according to §6 — not erased — and supersession relationships are preserved according to `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §6.5, so decision memory survives (Constitution §9).
- Change history is preserved as the appropriate governance record (Change Record, Decision Record) defined in `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`; this standard requires that history exist, not where it is technically stored.

## 14. Scope Boundaries

This standard governs document form and discipline. It does not own the content of any layer. The layers it serves are distinct:

- **Architecture** owns durable structure — boundaries, capabilities, information objects, roles, authorities, gates, interfaces. This standard governs how architecture documents are *written*, not what they define.
- **Standards** (this layer) own how work and documents are produced. A standard sets rules of form and practice; it does not decide architecture or execute work.
- **Playbooks** own repeatable guidance for performing studio work. A playbook applies architecture and standards to a recurring task; it does not define structure or governance.
- **ADRs** own the record of a single consequential decision and its rationale. An ADR captures a choice; it does not restate the architecture the choice operates within.
- **Implementation** owns the changing realization — specific procedures, artifacts, tools, and vendors. This standard is technology-neutral and defines nothing in implementation.

Where a document would blur these, the primary layer is declared and the others are referenced.

## 15. Known Unknowns

The following are explicitly unresolved and pending audit or later standards work; recorded as known unknowns, not assumptions:

- Whether existing VSOS documents already conform to this standard, and where they diverge.
- Which authority category is assigned as the standing Owner and Authority for each document class (pending the authority-assignment audit noted in `DECISION_CONTROL_ARCHITECTURE.md` §11).
- Whether additional document classes beyond those in §3 are needed as later layers are built.
- What the retention and deprecation cadence is for aged documents (Constitution Open Questions; §11 retention).
- Whether ADR, Playbook, and Agent Specification layers will require class-specific standard extensions.

These remain **[UNKNOWN]** until established through the change-control process.

---

## Self-Verification

- **No conflict with architecture.** This standard references the Constitution and the seven architecture documents by section and redefines none of them; where a fact is architectural, it points to the owning document.
- **No duplicated governance.** Authority, change control, source-of-truth, and truth-labeling are referenced from their authoritative homes (Constitution §4, §8, §10, §13; `DECISION_CONTROL_ARCHITECTURE.md`; `INFORMATION_KNOWLEDGE_ARCHITECTURE.md`), not restated as new governance.
- **No implementation leakage.** No tool, vendor, storage mechanism, repository layout, or workflow is defined; §9, §13, and §14 explicitly push those below the standard.
- **Suitable for every future VSOS document.** §2 and §3 cover all document classes, and §4–§13 apply uniformly across them, so the standard governs architecture, standards, ADRs, playbooks, agent specifications, and governance documents alike.

*Draft v0.1. A Standards-layer document governing how VSOS documents are written. Subordinate to the Constitution and consistent with the Core Architecture. Not self-ratifying; amendable only through change control.*

## ADR Standard

# VSOS ADR Standard

**Status:** Draft
**Version:** 0.1.0
**Type:** Standard — foundational
**Owner:** Architecture Steward (`HUMAN_AGENT_OPERATING_MODEL.md` §4.7) [TARGET — pending governance assignment]
**Authority:** Change Authority (`DECISION_CONTROL_ARCHITECTURE.md` §4.3) [TARGET — pending governance assignment]
**Precedence:** Subordinate to the Constitution; consistent with the Core Architecture; conforms to `DOCUMENTATION_STANDARD.md`.
**Last Updated:** [UNKNOWN — set on ratification]
**Related Documents:** `CONSTITUTION.md`; the seven Core Architecture documents in `docs/architecture/`; `DOCUMENTATION_STANDARD.md`.

## Preamble

This document defines how Architecture Decision Records (ADRs) are created, reviewed, approved, superseded, and archived in VSOS. It is a standard, not an architecture document: it governs the *form and governance of decision records*, not the decisions themselves and not the architecture those decisions operate within.

It conforms to `DOCUMENTATION_STANDARD.md` for all document form, metadata, versioning, and reference discipline, and adds only the rules specific to ADRs. Where it needs an architectural or governance fact, it references the authoritative document rather than restating it. If this standard conflicts with the Constitution or Core Architecture, those win, resolved through change control (Constitution §13).

---

## 1. Purpose

An ADR preserves a consequential decision so that a later reader understands what was decided, why, what was rejected, and under what conditions to revisit it. This standard exists so every such decision is recorded the same way and remains traceable.

It realizes the Constitution's decision discipline (§8) and the architecture's requirement that consequential architecture decisions be recorded (`ARCHITECTURE_OVERVIEW.md` §5). An ADR is the documentary form of the **Decision Record** information object (`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4.10); this standard governs that form.

## 2. Scope

This standard applies to every ADR authored in VSOS — decisions affecting architecture, standards, governance structure, or other controlled studio-level concerns.

It governs how ADRs are written and managed. It does not make the decisions, define who holds authority to approve them (that is `DECISION_CONTROL_ARCHITECTURE.md`), define repository mechanics, or introduce any tool or vendor. It is technology-neutral.

## 3. What Is an ADR

An ADR is a record of one consequential decision. It captures, at minimum: the decision, its context, the evidence the decision rests on, the assumptions the decision rests on, the hypotheses the decision rests on, the alternatives considered, the rationale, the consequences, and the conditions under which it should be revisited (Constitution §8). Evidence, assumptions, and hypotheses must be classified according to Constitution §4.

An ADR records a **single** decision. A record covering several unrelated decisions is split. An ADR is a decision record, not a design document, a specification, or a restatement of the architecture the decision operates within.

## 4. When an ADR Is Required

An ADR is required for any consequential, not-easily-reversible decision about studio-level structure or governance, including a decision that:

- Alters or resolves how a Core Architecture element is interpreted or applied (a boundary, capability, information object, role, authority, control gate, or interface).
- Creates, amends, or deprecates a standard.
- Chooses among materially different structural or governance options with lasting consequences.
- Resolves a conflict between authoritative documents or views.
- Establishes a durable convention that later work is expected to follow.

The test is consequence and reversibility (Constitution §8): decisions that are expensive or hard to reverse are recorded before they take effect.

## 5. When an ADR Is NOT Required

An ADR is not required for:

- Reversible, low-consequence choices with no lasting structural effect.
- Wording, clarification, or formatting changes that alter no owned element (handled as PATCH edits per `DOCUMENTATION_STANDARD.md` §5).
- Implementation choices — specific procedures, tools, or vendors — which belong to the implementation layer, not to an ADR.
- Restating or applying a decision already recorded; the existing ADR is referenced, not duplicated.
- Amending the Constitution itself, which follows the Constitution's own amendment process under Constitutional Authority (§13); an ADR may record a subordinate decision that flows from such an amendment, but does not substitute for it.

When in doubt, prefer recording: an unnecessary ADR is cheaper than an unrecorded consequential decision.

## 6. ADR Lifecycle

An ADR moves through recorded states, consistent with Constitution §13 (Audit → Design → Approval → Implementation) and the Decision Record lifecycle (`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4.10):

1. **Proposed** — the decision, its context, alternatives, and rationale are drafted for review. Not authoritative.
2. **Under review** — evaluated against authoritative documents by a reviewer distinct from the preparer (`DECISION_CONTROL_ARCHITECTURE.md` §3.5).
3. **Accepted** — approved by the authority with jurisdiction over the affected concern; the decision is in force and leaves the required governance records.
4. **Rejected** — not adopted; retained for traceability so the considered-and-declined option is preserved.
5. **Superseded** — replaced by a later ADR (§16); retained, not erased.
6. **Deprecated / Archived** — no longer in force or retained for history only, per `DOCUMENTATION_STANDARD.md` §6.

Movement between states is a discrete, recorded act by the governing authority, never implied by editing.

## 7. ADR Metadata

Every ADR carries the metadata block required by `DOCUMENTATION_STANDARD.md` §4, with ADR-specific fields:

- **Status** — one of the ADR statuses in §8.
- **Identifier** — the unique ADR identifier per §9.
- **Type / Class** — ADR.
- **Version** — maintained while the ADR document is Draft and set to `1.0.0` when the ADR reaches Accepted. After acceptance, the ADR remains at Version `1.0.0`; Version is no longer incremented, and any material change requires a new or superseding ADR according to §16.
- **Last Updated** — the date of the most recent approved change to the ADR document. Before acceptance it may change as the draft is revised. When the ADR reaches Accepted and Version `1.0.0`, it becomes fixed together with the accepted ADR. It is distinct from Date decided.
- **Owner** — the accountable role category (`HUMAN_AGENT_OPERATING_MODEL.md`); never a named individual.
- **Authority** — the authority category (`DECISION_CONTROL_ARCHITECTURE.md` §4) whose approval governs the decision.
- **Date decided** — the date the ADR reached Accepted; `[UNKNOWN]` until then.
- **Related Documents** — the authoritative documents the decision affects or depends on, and any ADR it supersedes or is superseded by.
- **Revisit conditions** — the conditions under which the decision should be reconsidered (Constitution §8).

## 8. ADR Status Model

An ADR carries exactly one status: **Proposed**, **Under review**, **Accepted**, **Rejected**, **Superseded**, **Deprecated**, or **Archived**, as defined in §6. ADR status is a specialized adjudication lifecycle. Documentation status governs the ADR as a document (`DOCUMENTATION_STANDARD.md` §6); Decision Record lifecycle governs the recorded decision (`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4.10).

| ADR Status | Document Status (`DOCUMENTATION_STANDARD.md` §6) | Decision Record Lifecycle (`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §4.10) |
| --- | --- | --- |
| Proposed | Draft | Proposed |
| Under review | Draft | Proposed |
| Accepted | Approved | Decided / Active |
| Rejected | Archived | Proposed, closed without adoption |
| Superseded | Deprecated | Superseded |
| Deprecated | Deprecated | Active but no longer recommended / retained |
| Archived | Archived | Archived |

Ratified has no ADR equivalent. Revisited is handled by confirmation or by a new superseding ADR. An ADR is never self-approving: Proposed is the default, and only the governing authority moves it to Accepted.

## 9. ADR Numbering and Identifiers

- Each ADR has a unique, stable, sequential identifier assigned when it is proposed.
- Identifiers are never reused, even for rejected or superseded ADRs, so references remain stable.
- A rejected or superseded ADR keeps its identifier and record; supersession links the old and new identifiers (§16).
- The identifier scheme is a naming convention under `DOCUMENTATION_STANDARD.md` §10; the exact format is a convention, not architecture, and remains technology-neutral.

## 10. Relationship With the Constitution

ADRs are subordinate to the Constitution and may not contradict it. An ADR records decisions *within* constitutional bounds; it never amends, reinterprets, or overrides the Constitution. Amending the Constitution is reserved to its own process under Constitutional Authority (§13). This standard does not redefine any constitutional rule; it references §4 and §8 as the source of decision and truth discipline.

## 11. Relationship With the Core Architecture

An ADR may record a decision that applies or interprets the Core Architecture, but it does not redefine architecture. A decision that changes an architecture element is an architecture change: it is approved by Architecture Authority and recorded both as the architecture document's versioned change and as its ADR (`ARCHITECTURE_OVERVIEW.md` §5). The ADR captures the decision; the architecture document remains the single source of truth for the element itself.

## 12. Relationship With Standards

An ADR may record the decision to create, amend, or deprecate a standard. The ADR preserves the *decision and rationale*; the standard remains the authoritative home for the *rule*. This ADR standard governs the form of such records; it does not itself decide any standard's content.

## 13. Relationship With Playbooks

An ADR may record a decision that establishes or changes a durable convention a playbook then follows. The ADR is the decision; the playbook is the repeatable guidance that applies it. An ADR does not contain playbook guidance, and a playbook does not substitute for the ADR that authorized its convention.

## 14. Relationship With Implementation

An ADR does not define implementation. Implementation owns the changing realization — procedures, artifacts, tools, vendors — beneath the decision. An ADR may constrain implementation by recording a structural or governance decision, but it never specifies implementation detail, and implementation choices do not require ADRs (§5).

## 15. Change-Control Rules

- Creating, accepting, rejecting, superseding, deprecating, or archiving an ADR follows Audit → Design → Approval → Implementation (Constitution §13).
- Approval comes from the authority with jurisdiction over the affected concern (`DECISION_CONTROL_ARCHITECTURE.md` §4); this standard does not redefine Change Authority or any other authority category — it references them.
- The preparer of an ADR is distinct from its approver (`DECISION_CONTROL_ARCHITECTURE.md` §3.5); an ADR is not approved by its author.
- Every state change leaves the governance records the control view requires (Decision Record, Authority Record, and where applicable Change Record).
- An accepted ADR is not silently edited. A material change to a decision is made by a new or superseding ADR, not by rewriting the original.

## 16. Superseding Previous ADRs

- A decision is changed by issuing a new ADR that explicitly supersedes the prior one, citing its identifier.
- The superseded ADR is marked Superseded (§8) and retained, never deleted, so decision memory survives (Constitution §9; `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §6.5).
- Supersession is bidirectional in reference: the old ADR points to the one that replaced it, and the new ADR points back to the one it replaced.
- Superseding an ADR that changed an architecture element is itself an architecture change and follows §11.

## 17. Cross-Reference Rules

- ADRs follow the cross-reference and citation rules of `DOCUMENTATION_STANDARD.md` §7 and §11: reference the single authoritative source, name document and section, never restate.
- An ADR references the architecture elements, standards, or prior ADRs it affects; it does not copy their content.
- References to a superseded or deprecated ADR are repointed or annotated through change control; dangling references are defects.

## 18. Known Unknowns

Recorded as known unknowns, not assumptions; pending audit or later standards work:

- Which authority category is assigned to approve each class of ADR (pending the authority-assignment audit in `DECISION_CONTROL_ARCHITECTURE.md` §9).
- Whether any decisions already made in existing work should be retroactively captured as ADRs.
- The concrete identifier format and any partitioning of ADR series (a convention to be fixed under `DOCUMENTATION_STANDARD.md` §10).
- Whether non-architecture decision classes will need ADR-standard extensions.

These remain **[UNKNOWN]** until established through change control.

## 19. Scope Boundaries

- **This standard owns:** the form, metadata, lifecycle, status model, numbering, supersession, and cross-reference discipline of ADRs.
- **The Constitution owns:** decision and truth discipline and the amendment process (§4, §8, §13).
- **`DECISION_CONTROL_ARCHITECTURE.md` owns:** the authorities and gates that approve decisions; this standard references them and defines none.
- **The Core Architecture documents own:** the architecture elements an ADR may decide about; the ADR references, never redefines.
- **`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` owns:** the Decision, Authority, and Change record objects an ADR produces.
- **`DOCUMENTATION_STANDARD.md` owns:** the general document rules this standard specializes.
- **Standards, Playbooks, and Implementation** own their respective content, as bounded in §12–§14.

Where a document would blur these, the ADR declares itself an ADR and references the rest.

## 20. Self-Verification

- **No architecture redefinition.** Architecture, information objects, roles, authorities, and gates are referenced by section; none is redefined. Decisions that change architecture route to Architecture Authority and the architecture document's own versioning (§11).
- **No implementation leakage.** No tool, vendor, format, repository mechanic, or workflow is defined; §14 and §9 push those below the standard.
- **No governance duplication.** Change control, authority, decision discipline, and record definitions are referenced from the Constitution, control view, and information architecture — not restated as new governance. Change Authority is referenced, not redefined (§15).
- **Suitable as the ADR standard for all future VSOS decisions.** §2–§6 cover when an ADR is and is not required and how it lives; §10–§14 place it correctly against every layer; §16–§17 keep decisions traceable over time — so the standard governs any consequential studio-level decision uniformly.

*Draft v0.1.0. A Standards-layer document governing how VSOS ADRs are created, reviewed, approved, superseded, and archived. Subordinate to the Constitution, consistent with the Core Architecture, conforming to the Documentation Standard. Not self-ratifying; amendable only through change control.*
