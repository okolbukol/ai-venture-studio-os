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
