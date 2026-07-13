# VSOS Documentation Standard

**Status:** Draft
**Version:** 0.1.0
**Type:** Standard — foundational
**Owner:** Architecture Authority (documentation governance)
**Authority:** Subordinate to the Constitution; consistent with the Core Architecture. Binds all VSOS documents.
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
- Prior authoritative versions are superseded, deprecated, or archived per §6 — not erased — so decision memory survives (Constitution §9; `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §6.5).
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
- **No implementation leakage.** No tool, vendor, format, storage mechanism, repository layout, or workflow is defined; §9, §13, and §14 explicitly push those below the standard.
- **Suitable for every future VSOS document.** §2 and §3 cover all document classes, and §4–§13 apply uniformly across them, so the standard governs architecture, standards, ADRs, playbooks, agent specifications, and governance documents alike.

*Draft v0.1. A Standards-layer document governing how VSOS documents are written. Subordinate to the Constitution and consistent with the Core Architecture. Not self-ratifying; amendable only through change control.*
