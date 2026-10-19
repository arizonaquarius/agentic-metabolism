# Agentic Metabolism

**Research into durable human context, inspectable evidence, and bounded agency.**

Agentic Metabolism (AM) asks how a person might preserve the history of their thinking across conversations, documents, models, and years — and eventually delegate useful work without surrendering control of consequential actions.

Two problems belong together:

- **Information continuity.** Where did a claim originate? Was it observed, inferred, disputed, or corrected? Can we reconstruct what was understood *at the time*, before later evidence arrived?
- **Governed action.** What does the person want? What may a model propose? What was authorized, within which limits, and what independent evidence tells us what actually happened?

A newer AI summary should not quietly replace original evidence. A persistent reminder should not become standing permission to act. A model reporting success is not the same thing as observing an effect.

AM is **early-stage research**. It is not an available personal assistant, a production security platform, or an unrestricted autonomous system.

## Why build it?

Digital systems preserve outcomes more readily than the paths that produced them. Conversations accumulate, objectives get lost, and interpretations are compressed into summaries. A mistaken synthesized memory may be repeated until it looks like established fact.

The longer-term ambition is a **personal cognitive interface**: an environment in which a person can revisit observations, inspect changes of mind, recover unfinished objectives, test competing interpretations, and enlist replaceable models and tools. The original evidence remains available for challenge and correction. The person remains responsible for intent and consequential authorization.

“Metabolism” is a working metaphor for retaining, interpreting, revising, and using information. It is not a claim to have solved memory or cognition.

[Read the research direction →](DIRECTION.md)

## Architectural separation

The architecture distinguishes information, proposals, authority, execution, and observation.

| Responsibility | Boundary |
| --- | --- |
| **Information plane** | Preserve evidence, attributed interpretation, corrections, and historical context. Information grants no execution rights. |
| **Proposal layer** | Models suggest actions and explain uncertainty. A proposal is not permission. |
| **Scoped authority** | A human or explicitly authorized principal decides which actions, lifetimes, and resources are allowed. |
| **Execution** | Work is constrained by reviewed interfaces and runtime boundaries, not assumed model obedience. |
| **Independent observation** | Record outcomes, resource use, failures, and uncertainty without treating an agent's self-report as proof. |

This is a conceptual map, **not** a complete implementation. AM is being developed from its evidence and authority boundaries outward, rather than beginning with a broad list of agent features.

## Evidence-backed progress

As of **October 19, 2026**, the latest promoted *private* implementation checkpoint is **v0.5.0**, focused on information-plane evidence continuity.

A fixed-input local prototype preserves source evidence, explicit interpretations, corrections, and reconstructable historical packets. Separate finite supervisor and qualification experiments exercise scoped authority, process observation, lifecycle behavior, accounting, and uncertainty.

This does **not** establish a general long-term memory service, autonomous interpretation of arbitrary documents, or production-ready containment. Generic hostile-workload admission remains closed. A planned hostile qualification campaign has not been executed, and a historical regression discrepancy remains unresolved despite successful later reruns.

[Read the research status and limits →](STATUS.md)

## Questions worth testing

- When a synthesized memory conflicts with original evidence, what should survive and how should the disagreement be represented?
- Can past decisions be reconstructed without importing facts learned later?
- Does curated, provenance-bearing context actually improve subsequent model reasoning?
- How can an objective remain available for years without becoming indefinite authority?
- What would count as independent evidence that an external action occurred, failed, or remains uncertain?
- Can personal context and intent remain portable when the provider, model, or interface changes?

Personal research, technical work, and evidence-aware financial analysis are possible application domains. This does not imply automatic brokerage or wallet activity.

## Defensive research and publication boundary

Security properties are hypotheses until tested against specific invariants. Adversarial validation is limited to owned or expressly authorized test environments. Untrusted workloads are research specimens, not the intended ordinary operation of an assistant.

This public repository is a **separately authored description**, not a mirror of the private codebase. Detailed implementation, test evidence, machine configuration, credentials, and personal material remain private. The internal results described here cannot be reproduced from the public repository alone.

**Start here:** [DIRECTION.md](DIRECTION.md) for the long-term ambition; [STATUS.md](STATUS.md) for what has and has not been demonstrated.

**License:** No project license has been selected.
