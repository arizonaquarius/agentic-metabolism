# Agentic Metabolism

**Research into durable personal context, independent operational tools, and bounded agency.**

Agentic Metabolism (AM) is an experimental personal institution: a system for preserving the history of a person's thinking and work across conversations, documents, models, and years, and making that experience useful in subsequent decisions and operations.

Three complementary concerns shape the project:

- **Information continuity.** Where did a claim originate? Was it observed, inferred, disputed, or corrected? Can we reconstruct what was understood *at the time*, before later evidence arrived?
- **Operational competence.** What can dependable, independently usable tools collect, transform, verify, maintain or recover without needing a reasoning model?
- **Governed action.** What does the person want? What may a model propose? What was authorized, within which limits, and what independent evidence tells us what actually happened?

A newer AI summary should not quietly replace original evidence. A persistent reminder should not become standing permission to act. A model reporting success is not the same thing as observing an effect.

AM is an **early-stage research and development project**. Small working components coexist with unfinished integration and architectural experiments. It is not a publicly available personal assistant, a production security platform, or an unrestricted autonomous system.

## Why build it?

Digital systems preserve outcomes more readily than the paths that produced them. Conversations accumulate, objectives get lost, and interpretations are compressed into summaries. A mistaken synthesized memory may be repeated until it looks like established fact.

The longer-term ambition is a **personal cognitive interface**: an environment in which a person can revisit observations, inspect changes of mind, recover unfinished objectives, test competing interpretations, and enlist replaceable models and tools. The original evidence remains available for challenge and correction. The person remains responsible for intent and consequential authorization.

“Metabolism” is a working metaphor for the circulation and transformation of information and work: experience is preserved, relevant context is recovered, tools and people perform operations, outcomes are observed, and the record grows. It is not a claim to have solved memory or cognition.

A useful institution should retain not only its successes, but the difficulties, failed attempts, corrections, unresolved work and the person's own account of why an outcome mattered. Such case histories are revisable interpretations linked to evidence, not replacements for the sources. Practical outcomes, reduced repetitive effort and demonstrated recovery matter more than agent activity or the volume of generated reports.

[Read the research direction →](DIRECTION.md)

## Architectural separation

Four logical components express different responsibilities. They are not four required running services or a completed package migration.

| Component | Intended responsibility |
| --- | --- |
| **am-core** | Institutional continuity and learning: task-scoped context assembly from preserved experience, interpretation, persistent intent and governance. |
| **am-utilities** | Independently useful deterministic tools for retrieval, collection, transformation, verification and routine work. |
| **am-phygitals** | Preservation, provenance, controlled archival acceptance, custody and recovery. |
| **am-glass** | Human-facing inspection of evidence, decisions, proposals and operational state. |

Core and Utilities are complementary, not a hierarchy of importance. The ability to understand the circumstances of a task is distinct from the ability to perform it reliably. A utility should remain usable by the person or an authorized agent without requiring Core or a model to run. In turn, operational evidence can inform Core's later investigations and help improve the tools.

The architecture also distinguishes information, proposals, authority, execution, and observation. These are boundaries across components, rather than additional mandatory services.

| Responsibility | Boundary |
| --- | --- |
| **Information plane** | Preserve evidence, attributed interpretation, corrections, and historical context. Information grants no execution rights. |
| **Proposal layer** | Models suggest actions and explain uncertainty. A proposal is not permission. |
| **Scoped authority** | A human or explicitly authorized principal decides which actions, lifetimes, and resources are allowed. |
| **Execution** | Work is constrained by reviewed interfaces and runtime boundaries, not assumed model obedience. |
| **Independent observation** | Record outcomes, resource use, failures, and uncertainty without treating an agent's self-report as proof. |

This is a conceptual map, **not** a complete implementation. Prefer deterministic operations and known failure handling; introduce bounded model judgment when evidence conflicts, a problem is novel, or a choice among tools warrants interpretation. Keep durable methods and identities separate from replaceable mechanisms. A named institutional responsibility does not require a dedicated daemon, database or agent.

## Evidence-backed progress

As of **November 25, 2026**, the documented promoted *private* implementation checkpoint remains **v0.5.0**, focused on information-plane evidence continuity.

A fixed-input local prototype preserves source evidence, explicit interpretations, corrections, and reconstructable historical packets. Separate finite supervisor and qualification experiments exercise scoped authority, process observation, lifecycle behavior, accounting, and uncertainty.

Subsequent merged development adds bounded local file inventories, source-preserving transaction-export analysis and snapshot comparison, and a local read-only **Glass** browsing demo. Glass uses conspicuously fictional records; it is not connected to financial accounts or an archival service. A subsequent reviewed change adds a restricted service template and a commit-pinned Glass deployment and rollback procedure; local verification and rehearsal are recorded, while target-host and physical-device acceptance remain unestablished in the reviewed record. These are small implemented slices after the checkpoint, not a new promoted release or a deployed assistant.

Broader archival services, general corpus ingestion and selective context assembly, institutional case-history retrieval, shared workers, live integrations and operational Agent Authority Contract enforcement remain proposed or partial. The research direction is informed by actual personal workflows, but their individual successes do not establish an integrated AM system. [STATUS.md](STATUS.md) distinguishes **DEMONSTRATED**, **PARTIAL**, **PROPOSED** and **UNRESOLVED** work.

This does **not** establish a general long-term memory service, autonomous interpretation of arbitrary documents, or production-ready containment. Generic hostile-workload admission remains closed. A planned hostile qualification campaign has not been executed, and a historical regression discrepancy remains unresolved despite successful later reruns.

[Read the research status and limits →](STATUS.md)

## Questions worth testing

- When a synthesized memory conflicts with original evidence, what should survive and how should the disagreement be represented?
- Can past decisions be reconstructed without importing facts learned later?
- Does curated, provenance-bearing context actually improve subsequent model reasoning, and can retrieval reconstruct relevant conversation branches without losing chronology or duplicating shared history?
- Can a tool remain useful without a model or central runtime? When does an unresolved operational problem warrant agentic investigation?
- Can a case history preserve the struggle and the person's own assessment of an outcome without conflating them with independently measured results?
- How can an objective remain available for years without becoming indefinite authority?
- What would count as independent evidence that an external action occurred, failed, or remains uncertain?
- Can personal context and intent remain portable when the provider, model, or interface changes?

Personal research, technical work, and evidence-aware financial analysis are possible application domains. This does not imply automatic brokerage or wallet activity.

## Defensive research and publication boundary

Security properties are hypotheses until tested against specific invariants. Adversarial validation is limited to owned or expressly authorized test environments. Untrusted workloads are research specimens, not the intended ordinary operation of an assistant.

This public repository is a **separately authored description**, not a mirror of the private codebase. Detailed implementation, test evidence, machine configuration, credentials, and personal material remain private. The internal results described here cannot be reproduced from the public repository alone.

**Start here:** [DIRECTION.md](DIRECTION.md) for the long-term ambition; [STATUS.md](STATUS.md) for what has and has not been demonstrated.

**Documentation license:** The original text in this public README, [DIRECTION.md](DIRECTION.md), and [STATUS.md](STATUS.md) is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE-DOCS.md). Reuse and adaptation are welcome with appropriate attribution. The grant covers the specified public documentation, not implementation code, private research artifacts, or third-party material.

**Software license:** Not yet selected. A future public software release may be open-source under a separately chosen software license.
