# VSOS Review Standard

**Status:** Draft
**Version:** 0.1.0
**Type:** Standard
**Owner:** Architecture Steward [TARGET — pending governance assignment] (`HUMAN_AGENT_OPERATING_MODEL.md` §4.7)
**Authority:** Change Authority [TARGET — pending governance assignment] (`DECISION_CONTROL_ARCHITECTURE.md` §4.3)
**Last Updated:** [UNKNOWN — set on ratification]
**Precedence:** Subordinate to the Constitution; consistent with the Core Architecture; conforms to `DOCUMENTATION_STANDARD.md`.
**Related Documents:** `CONSTITUTION.md`; the seven Core Architecture documents in `docs/architecture/`; `DOCUMENTATION_STANDARD.md`; `ADR_STANDARD.md`.

## Preamble

This document defines how every VSOS document is independently reviewed before approval. It is a standard, not an architecture document: it governs the *conduct and record of review*, not the authority that approves, the gates a change passes, or the content of any document reviewed.

It conforms to `DOCUMENTATION_STANDARD.md` for all document form, metadata, versioning, and reference discipline. Where it needs a governance or architectural fact, it references the authoritative document rather than restating it. If this standard conflicts with the Constitution or the Core Architecture, those win, resolved through change control (Constitution §13).

---

## 1. Purpose

Approval must rest on evidence, not assertion (`DECISION_CONTROL_ARCHITECTURE.md` §3.3). Review is how that evidence is produced: it is the independent examination on which an approving authority relies when moving a document from Draft to Approved (`DOCUMENTATION_STANDARD.md` §6).

This standard exists so that review is conducted the same way every time, by someone other than the author, against the authoritative documents rather than against preference, and so that it leaves a record a later reader can trust.

Review is not approval. A review produces a verdict and findings; the authority with jurisdiction decides (`DECISION_CONTROL_ARCHITECTURE.md` §4). This standard defines the former and references the latter.

## 2. Scope

This standard applies to the review of every VSOS document class defined in `DOCUMENTATION_STANDARD.md` §3 — Constitution, Architecture, Standard, ADR, Playbook, Agent Specification, governance document, and repository documentation.

It governs how review is conducted, classified, and recorded. It does not decide anything, does not define who holds approval authority, does not define control gates or escalation (`DECISION_CONTROL_ARCHITECTURE.md`), does not define the content of any document reviewed, and introduces no tool, vendor, or mechanism. It is technology-neutral.

## 3. Review Principles

These principles constrain every review. Each traces to the authoritative architecture.

1. **Independence.** The reviewer is distinct from the preparer. Preparation is never approval, however accurate (`DECISION_CONTROL_ARCHITECTURE.md` §3.5).
2. **Evidence before approval.** A review judges the document as it actually is, against the authoritative set. No verdict is issued on assertion, recollection, or expectation (`DECISION_CONTROL_ARCHITECTURE.md` §3.3).
3. **Judge against the authoritative set, not against preference.** A document is measured against the Constitution, Core Architecture, and applicable standards — never against the design the reviewer would have chosen. A preference is not a finding.
4. **Truth over deference.** Defects are stated plainly and completely. A verdict is not a courtesy, and agreement is not a review outcome (Constitution §3.7).
5. **Conservatism.** Architectural stability is preferred over improvement. Where correction is required, the minimum correction is specified (`ARCHITECTURE_OVERVIEW.md` §2, principle 6).
6. **Review only what is present.** If the document under review is absent, incomplete, or unverifiable, the review does not proceed and the gap is recorded. Nothing is reconstructed, assumed, or invented to complete a review (Constitution §4).
7. **Scope discipline.** The review examines the document under review. Its authoritative inputs are treated as authoritative and are not reviewed in the same pass.
8. **Classification discipline.** Every finding carries exactly one classification (§8). An unclassified observation is not a finding.
9. **Auditability.** Every review leaves a record sufficient for a later reader to understand what was reviewed, against what, by whom, and with what result (`DECISION_CONTROL_ARCHITECTURE.md` §3.7).

## 4. Reviewer Independence

- The reviewer is a role category distinct from the role that prepared the document (`HUMAN_AGENT_OPERATING_MODEL.md` §4.4; `DECISION_CONTROL_ARCHITECTURE.md` §3.5).
- **Independence is a structural property, not an intention.** An author does not become independent by reviewing rigorously, disclosing bias, or trying to be objective. Independence is determined by who prepared the document, not by how carefully it is examined.
- Reviewing confers no authority. A reviewer may recommend; only the authority with jurisdiction approves (`HUMAN_AGENT_OPERATING_MODEL.md` §3.1).
- An AI agent role may perform a review as preparation of evidence for a human authority, and may never approve, and may never review a document it prepared (Constitution §7).
- Where independence cannot be achieved, the review is disclosed as non-independent and is treated as a self-review under §10. Absence of an available independent reviewer is not grounds to waive independence; it is a gap to record and a reason to defer approval.

## 5. Review Inputs

A review requires, at minimum:

- **The document under review**, complete, as it actually exists, at a stated version.
- **The authoritative documents** it must be judged against — the Constitution, the applicable Core Architecture documents, and the applicable standards.
- **The document's declared class, status, and metadata** (`DOCUMENTATION_STANDARD.md` §3, §4, §6).
- **The review criteria** applicable to that class.

Rules of input:

- Inputs are treated as authoritative and are not themselves reviewed in the pass (§3.7).
- If the document under review is missing, truncated, or otherwise not fully available, the review does not proceed. The condition is recorded as a blocking finding and no verdict is issued (§3.6).
- A review is performed against a stated version; a review of an unstated or unstable version is not auditable.

## 6. Review Outputs

Every completed review produces:

- Exactly **one verdict** (§7).
- **Findings**, each classified (§8), with the minimum correction required for each blocking finding.
- An **independence disclosure** stating whether the review was independent (§4) or a self-review (§10).
- A **review record** (§12).

A review does not produce an approval, a version change, an amended document, or a redesign. Corrections are specified; applying them is the preparer's act, and accepting them is the authority's.

## 7. Review Verdicts

A review issues exactly one verdict, describing the document's conformance state:

- **PASS** — the document conforms to the authoritative set. No corrections are required. Suggestions may accompany a PASS.
- **PASS WITH COMMENTS** — the document conforms and is approvable as-is. Findings exist but none block approval; corrections are optional and at the authority's discretion.
- **FAIL** — the document does not conform. One or more findings block approval; the document is not approvable until they are resolved.

Rules of verdict:

- The verdict follows from the findings, per the thresholds in §8. A verdict inconsistent with its findings is a defect in the review.
- **A verdict is not an approval.** It is evidence for the authority that approves (`DECISION_CONTROL_ARCHITECTURE.md` §4). A PASS does not make a document Approved; the authority's recorded act does (`DOCUMENTATION_STANDARD.md` §6).
- A verdict is issued only on a document actually inspected in full (§5).
- FAIL is not a judgment on the work's value. It states that corrections are required before approval; the document returns to Draft, is corrected, and is re-reviewed (§11).

## 8. Finding Classifications

Every finding carries exactly one classification.

- **Critical** — violates the Constitution, contradicts the Core Architecture, or rests on fabricated or unverifiable content. Blocks approval unconditionally.
- **Major** — a substantive defect that would mislead a reader or propagate error: a broken authoritative reference, a missing required element, ambiguous ownership, an unsubstantiated claim of conformance, or scope leakage across a defined layer. Blocks approval until resolved.
- **Minor** — a defect that does not mislead: wording, a non-authoritative inconsistency, an incomplete but unambiguous reference. Does not block approval.
- **Suggestion** — an observation, an option, or a matter to carry forward. Never blocks, and is never a redesign request (§3.3).

Verdict thresholds:

| Findings present | Verdict |
|---|---|
| Suggestions only, or none | PASS |
| One or more Minor; no Critical or Major | PASS WITH COMMENTS |
| One or more Critical or Major | FAIL |

Classification is judged by consequence, not by tone or effort. A defect is not downgraded because it is easy to fix, nor upgraded because it is difficult.

## 9. Review Methodology

Methodology here means the dimensions and order of judgment, not a procedure. Sequencing, routing, and mechanism are implementation (§15).

A review establishes, in this order:

1. **Input completeness** — is the document fully present at a stated version (§5)? If not, the review stops.
2. **Class and metadata conformance** — does the document declare one class and carry the required metadata, with Owner as a role category and Authority as an authority category (`DOCUMENTATION_STANDARD.md` §3, §4)?
3. **Constitutional consistency** — does anything contradict the Constitution? The Constitution is judged first because it wins every conflict.
4. **Architectural consistency** — does anything contradict the Core Architecture, or redefine what another document authoritatively owns?
5. **Single-source-of-truth compliance** — is every fact referenced to its one authoritative home rather than restated (Constitution §10)?
6. **Scope discipline** — does the document stay inside its layer, without absorbing architecture, governance, or implementation that belongs elsewhere (`DOCUMENTATION_STANDARD.md` §14)?
7. **Internal consistency** — do the document's own sections, references, and claims agree with each other? A claim of conformance that the document does not substantiate is itself a defect.
8. **Truth-labeling** — are `[CURRENT]`, `[TARGET]`, and `[UNKNOWN]` used correctly, and is nothing unaudited presented as current (`DOCUMENTATION_STANDARD.md` §12)?
9. **Cross-reference integrity** — does every reference resolve to a section that exists in the document cited?
10. **Technology neutrality** — is the document free of tools, vendors, protocols, and implementation mechanics where its layer requires it?
11. **Completeness** — does the document contain the elements its class and purpose require?

The reviewer then classifies each finding (§8), issues one verdict (§7), and states the minimum correction for each blocking finding. The reviewer does not rewrite the document.

## 10. Self-Review Limitations

- A **self-review** is an examination performed by the party that prepared the document. It is a preparer's check, not a review.
- A self-review **cannot support approval**, regardless of its rigor, its verdict, or the absence of any other reviewer. Approval resting on a self-review collapses preparation and approval into one party, which the control architecture prohibits (`DECISION_CONTROL_ARCHITECTURE.md` §3.5).
- A self-review is nonetheless useful and is not discouraged: it surfaces defects early, at the preparation stage where correction is cheapest. It is recorded as preparation evidence, not as review evidence.
- A self-review is **explicitly disclosed as such** in its output and record. A self-review presented, labeled, or relied upon as an independent review is a Critical defect.
- Where a self-review is the only examination available, the document remains in Draft and the missing independent review is recorded as a known gap.

## 11. Re-Review Rules

- A **FAIL** requires correction and a new review before approval. The corrected document is reviewed again; the prior verdict does not carry forward.
- A re-review confirms that each blocking finding is resolved, and examines whether the corrections introduced new defects. Corrections are not assumed correct because they were requested.
- A re-review issues its own verdict and its own record. It does not amend, replace, or erase the prior review record; prior records are retained (Constitution §9; `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` §6.5).
- Independence rules apply to every re-review (§4). A reviewer who reviewed a prior version but did not author the document remains independent.
- **Disputed findings.** A preparer may dispute a finding. A dispute is not resolved by the reviewer or the preparer asserting the point; it is escalated to the authority with jurisdiction, whose resolution is recorded (`DECISION_CONTROL_ARCHITECTURE.md` §7). A finding may be accepted while its proposed remedy is rejected; the accepted defect must still be resolved.
- Findings accepted but deliberately not resolved are recorded as accepted defects with rationale, not silently dropped.

## 12. Review Records

Every review leaves a record containing, at minimum:

- The document reviewed and the version reviewed.
- The authoritative inputs it was judged against.
- The verdict (§7).
- Every finding, with its classification and, for blocking findings, the minimum correction required.
- The independence disclosure (§4, §10).
- The reviewer's role category and the date.

Rules of record:

- The review record is the evidence an approving authority relies on; authority is exercised only against evidence, and its exercise leaves its own record (`DECISION_CONTROL_ARCHITECTURE.md` §6). The review record and the authority's Decision or Authority Record are distinct and both are retained.
- Review records are preserved, never erased, including records of FAIL verdicts and disputed findings (Constitution §9).
- Where the review's outcome requires a consequential decision — for example, resolving a disputed finding structurally — that decision is recorded as an ADR (`ADR_STANDARD.md` §4). A review record is not an ADR.
- The record's format, location, and storage are implementation (§15).

## 13. Relationship With the Documentation Standard

`DOCUMENTATION_STANDARD.md` owns document form: classification, metadata, versioning, status, cross-reference, terminology, and unknowns. This standard governs how conformance to those rules is verified, and defines none of them.

The Draft → Approved transition (`DOCUMENTATION_STANDARD.md` §6) is the transition review informs: review supplies the evidence, the authority performs the act. Review never changes a document's status by itself.

## 14. Relationship With the ADR Standard

`ADR_STANDARD.md` owns ADR form and lifecycle, including the **Under review** status (§6, §8). This standard defines what review means while an ADR occupies that state; it does not define the ADR lifecycle.

ADRs are reviewed under this standard like any other document class, judged additionally against the ADR-specific requirements that `ADR_STANDARD.md` owns. A review is not itself an ADR: a verdict records a conformance judgment, not a decision. Where review outcomes require a decision, the decision is recorded per `ADR_STANDARD.md`.

## 15. Scope Boundaries

- **This standard owns:** review principles, independence, inputs and outputs, verdicts, finding classifications, methodology dimensions, self-review limits, re-review rules, and review records.
- **The Constitution owns:** truth and evidence discipline (§4), decision discipline (§8), preservation (§9), and change control (§13).
- **`DECISION_CONTROL_ARCHITECTURE.md` owns:** the authority categories, control gates, and escalation that review informs. Review never approves, never gates, and never escalates on its own authority.
- **The Core Architecture documents own:** the structure a reviewed document must conform to.
- **`INFORMATION_KNOWLEDGE_ARCHITECTURE.md` owns:** the information objects a review's evidence and resulting decisions are recorded as.
- **`DOCUMENTATION_STANDARD.md` and `ADR_STANDARD.md` own:** document form and ADR form, as bounded in §13 and §14.
- **Implementation owns:** the mechanism of review — sequencing, routing, notification, record storage and format, and any tool. This standard defines none.

## 16. Known Unknowns

Recorded as known unknowns, not assumptions; pending audit or later work:

- Which authority category approves each document class, and therefore which authority a review's evidence is addressed to (pending the authority-assignment audit in `DECISION_CONTROL_ARCHITECTURE.md` §9).
- Which role categories are eligible to serve as independent reviewer for each document class.
- Whether `INFORMATION_KNOWLEDGE_ARCHITECTURE.md` requires a Review Record information object, or whether review records are carried within existing objects. This standard requires the record to exist and does not define the object.
- Whether any existing VSOS document was approved on a self-review or without an independent review, and what remediation that requires.
- Whether class-specific review criteria extensions are needed beyond §9.
- Whether approved documents require re-review on a cadence, and what that cadence is.

These remain **[UNKNOWN]** until established through change control.

## 17. Self-Verification

- **No constitutional or architectural redefinition.** Truth discipline, decision discipline, preservation, change control, authorities, gates, escalation, information objects, and role categories are referenced by section; none is redefined.
- **No governance duplication.** Approval, authority, and escalation remain owned by `DECISION_CONTROL_ARCHITECTURE.md`; this standard states only that review produces evidence for them (§1, §7, §15).
- **No implementation leakage.** No tool, vendor, protocol, format, storage mechanism, or routing sequence is defined; §9 and §15 explicitly push those below the standard.
- **Technology-neutral.** The standard describes principles, roles, and records only, and names no product, platform, or model.
- **Suitable as the review standard for every VSOS document class.** §2 covers all classes in `DOCUMENTATION_STANDARD.md` §3; §3–§12 apply uniformly across them; §13–§14 place the standard correctly against its sibling standards.

*Draft v0.1.0. A Standards-layer document governing how VSOS documents are independently reviewed before approval. Subordinate to the Constitution, consistent with the Core Architecture, conforming to the Documentation Standard. Not self-ratifying; amendable only through change control.*
