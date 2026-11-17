# Research status and claim boundaries

*Public statement as of November 16, 2026. The implementation and detailed verification record are private. This document is not a security certification or a reproducible release package.*

## Current checkpoint

The latest promoted internal checkpoint is **v0.5.0**, focused on *information-plane evidence continuity*. It extends a separately developed research supervisor and qualification substrate with a local, fixed-input information store.

This is a bounded engineering result. It is not a deployed cognitive assistant, a generally secure sandbox, or an end-to-end agent that can perform external actions on a user's behalf.

Workload numbers record the history of research experiments; release tags mark promoted internal checkpoints. They are not equivalent to progressively increasing authority or assurance.

## Demonstrated work — with qualifications

| Area | What the private research demonstrates | What it does **not** establish |
| --- | --- | --- |
| **Evidence continuity** | Explicit source evidence, interpretations, mappings, corrections, and reconstructable historical packets in a local fixed-input prototype. | Autonomous acquisition, arbitrary document parsing, universal historical recall, source authenticity, or a system that decides semantic truth. |
| **Scoped authority** | Finite fixtures involving synthetic authorization, accounting, receipts, and lifecycle states in a reviewed supervisor interface. | Real-user authentication, universal permissions, production readiness, or permission to use outside accounts. |
| **Independent observations** | Named process and effect observations within tested conditions; failures and unknown effect states are retained. | Complete observation of every process, complete resource accounting, or reliable exactly-once external effects. |
| **Adversarial qualification** | A WL16 finite qualification substrate with **51 named fixtures** and defined evidence/claim structures. | Generic hostile-code admission. A planned hostile campaign remains **not executed**. |
| **Reproduction and review** | Recorded finite regressions and checkpoint verification for named source revisions, with output/evidence retention. | A successful run explaining every historical failure or proving safety outside the tested conditions. |

The information-plane prototype also includes a bounded experiment using reviewed real-world source material. Its inputs and semantic mappings were supplied, not autonomously extracted or independently authenticated by AM. The human semantic-review limitation remains explicit.

## Merged development after the checkpoint

The latest promoted checkpoint remains **v0.5.0**. The following separates subsequent merged capabilities from partial components, proposals and unresolved questions; no new release is implied:

| Status | Work and evidence boundary |
| --- | --- |
| **DEMONSTRATED** | Selected synthetic local files can be inventoried and hashed with deterministic content records and separate observation metadata. This is not a completed personal archive, transfer, backup or restoration system. |
| **DEMONSTRATED** | Local analysis preserves supplied transaction-export bytes and source rows, produces capture-bounded reports, and compares two explicitly selected snapshots. Missing capture evidence and ambiguous identities remain unresolved; reports do not establish settlement or an authoritative personal ledger. |
| **DEMONSTRATED** | A local read-only Glass demo supports browsing overview, obligation, observation and evidence views, with navigation regressions and targeted browser checks. Every example is fictional; no live account or archive is connected. |
| **PARTIAL** | Information continuity, inventory, financial analysis and presentation each have working local components. End-to-end acquisition, independently verified archival promotion, deployment and recovery are not established by combining those components. |
| **PROPOSED** | Four logical roles for reasoning, presentation, archival custody and shared computation, together with an Agent Authority Contract separating a Work Order, bounded grant and Result/Evidence Packet. No functional AAC executor or general browser agent is established. |
| **UNRESOLVED** | Production identity and grant enforcement, credential custody, real-clock expiry and revocation, archive acceptance and recovery, hostile containment, and the retained regression discrepancy. |

The Glass browser checks are limited emulation and interaction evidence, not physical-device, assistive-technology or complete accessibility certification. The public repository contains no private implementation or underlying test artifacts.

## Important unresolved boundaries

**Containment is incomplete.** The inherited operative containment baseline remains WL14-derived. Its reviewed-fixture path is not an open admission interface for arbitrary hostile workloads. No WL15 experimental containment mechanism has been promoted merely because it was attempted.

**Prepared tests are not executed tests.** The T01–T29 hostile qualification plan is represented in the internal record as `PREPARED_NOT_EXECUTED`. WL17/Daybreak remains separately gated research requiring reviewed controls, prerequisites, and authorization.

**A regression discrepancy remains unexplained.** One discovery-order baseline verification produced a fail-closed discrepancy, while isolated and later complete reruns succeeded. Its cause remains `UNRESOLVED_CAUSE`. Passing a rerun does not retroactively resolve it.

**Unknown effects remain unknown.** For irreversible external effects, a local receipt cannot always prove that an operation did or did not happen. Independent reconciliation and any retry need their own authority boundary.

**Historical interpretation is contextual.** A corrected observation need not overwrite an earlier packet. The prototype preserves lineage for specific fixed inputs. It does not establish complete public-availability dating, universally accurate interpretation, or the truth of an attributed claim.

These limitations are part of the research record, not incidental footnotes.

## Future research, not current capability

The project is exploring or considering:

- A source-preserving personal conversation and document corpus, with longitudinal retrieval and contradiction handling.
- Evaluation of context selection and historical reconstruction, including explicit tests of **with-context versus without-context** reasoning.
- A human-facing cognitive interface to examine associations, decisions, dissent, corrections, and unresolved questions.
- Long-lived objectives that can surface a useful next step without automatically extending the authority previously granted.
- Portable context across replaceable models and tools.
- More rigorous empirical security and containment qualification under controlled, authorized conditions.
- Research pilots, potentially including financial information, without claiming automated trading or privileged wallet/brokerage action.

None of these should be described as a shipped feature merely because it has been discussed, prototyped in another system, or represented in a visual design.

## Reading claims accurately

AM uses five distinctions:

- **Demonstrated:** a specific behavior was implemented and observed under stated conditions.
- **Partial:** some mechanisms exist but material obligations remain open.
- **Proposed:** the idea or experiment is described but not verified as an implementation.
- **Unresolved:** conflicting or anomalous evidence remains without an established explanation.
- **Unknown:** the available observations do not establish a fact or effect.

Source material, review bundles, diagrams, tests, and user conversations play different roles. Evidence supports a proposition only within its recorded scope. Neither a release label nor an elegant visual expands the trust boundary.

## Publication and security

This public repository is **not a mirror** of the private implementation. It intentionally excludes implementation source, sensitive adversarial test material, credentials, operational details, machine-specific environment information, and personal conversation corpora.

Defensive testing is restricted to owned or expressly authorized systems and controlled environments. The project does not advocate unauthorized access to third-party systems or claim that its adversarial research is suitable for ordinary production operation.

For the wider research thesis, read [DIRECTION.md](DIRECTION.md). For the entry point, return to [README.md](README.md).

---

*Public documentation licensed under [CC BY 4.0](LICENSE-DOCS.md). Software and private implementation remain separately licensed or unlicensed.*
