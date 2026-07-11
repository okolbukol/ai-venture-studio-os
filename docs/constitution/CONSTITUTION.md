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
