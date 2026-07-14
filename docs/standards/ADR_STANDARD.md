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