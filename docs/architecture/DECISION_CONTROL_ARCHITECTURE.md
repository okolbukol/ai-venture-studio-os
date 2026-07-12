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

The transition from Build to Growth is governed through the existing architectural control structure by the Build-Readiness Gate together with the recurring Portfolio-Review Gate.

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
