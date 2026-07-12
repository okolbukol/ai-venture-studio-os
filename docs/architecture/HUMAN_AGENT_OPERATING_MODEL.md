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
