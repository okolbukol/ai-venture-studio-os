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
