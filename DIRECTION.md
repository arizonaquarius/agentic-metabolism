# Research direction

*Agentic Metabolism · Working research thesis · October 19, 2026*

Agentic Metabolism (AM) is an attempt to connect two forms of continuity: a person's evolving understanding of the world, and their authority over software that helps them act in it.

Neither should depend on a single model being correct, cooperative, or available indefinitely. This document describes where the project is trying to go, not what it already delivers. See [STATUS.md](STATUS.md) for the evidence boundary.

## A record of thinking, not a personality summary

A decision rarely begins with a tidy question and ends with a final answer. It develops through observations, corrections, associative jumps, missed objectives, changing information, and decisions made with incomplete knowledge.

Most digital systems retain outputs more readily than the path that produced them. AI summaries compound the problem: an inference can become a remembered fact, then serve as a premise for new inferences. A later correction may overwrite the earlier account without preserving why the conclusion changed.

AM's ambition is to preserve enough of that history to ask:

- What did the person actually say, observe, or decide?
- What was an external source, and what was a model's interpretation of it?
- What information was available *at the time*?
- What contradictory evidence or later corrections exist?
- Which conclusion remains disputed, and why?

A synthesized memory should be challengeable against its sources. When an AI-generated recollection disagrees with an original conversation, the system should expose the conflict, not quietly elect a winner. Historical reconstruction is not the same as generating the most plausible current story.

The desired result is **epistemic continuity**: the ability to examine the ancestry of an understanding. It is not perfect recall, and it is not a claim that AM can independently determine what is true.

## Why “metabolism”?

The name is a metaphor for an inspectable transformation cycle:

1. **Ingest:** preserve raw material with source identities and dates.
2. **Interpret:** record claims, mappings, limits, competing readings, and uncertainty.
3. **Reconcile:** retain corrections, challenges, and the lineage of changed conclusions.
4. **Circulate:** assemble task-relevant context without stripping away epistemic distinctions.
5. **Propose:** let models suggest actions or experiments without conferring permission.
6. **Authorize and observe:** require separately scoped authority for consequential actions; distinguish their independently observed effects from claims of completion.

Not every stage has been implemented. A useful cognitive interface will need to help a person inspect and revise this process, rather than hide it behind an apparently seamless assistant.

## Long-horizon intent and human agency

A great deal of unfinished work is lost to divided attention, changing priorities, and the simple passage of time. AM might preserve the reason an objective was created and the conditions under which it should be reconsidered.

For example, an assistant might remember that a person wanted to evaluate an expiring subscription. Recovering the original motivation, reviewing new terms, and drafting a recommendation are different from canceling an account or accepting an offer. The earlier intention is not standing permission to act.

This distinction gets sharper as agents work across websites, local files, financial accounts, and organizations with their own policies. An agent should be useful even when it cannot execute a task. It can preserve the user's goal, record the obstruction, and propose a reviewable alternative.

The aim is to increase an individual's leverage and continuity, not replace their judgment or make automation an end in itself.

## The architecture follows from that separation

AM distinguishes:

- **Information:** observations, documents, conversation records, interpretations, contradictions, and provenance.
- **Proposals:** model-generated candidate actions with uncertainty and stated assumptions.
- **Authority:** explicitly permitted actions with bounded scope, time, resource budgets, and revocation conditions.
- **Execution:** a controlled runtime whose capabilities cannot be inferred merely from what software can reach.
- **Independent observation:** evidence about what happened, including failures, cleanup, and unresolved effect states.

An information packet is not an authority token. A model's assertion of success is not independent observation. A known deadline is not consent to spend money. These boundaries remain important even when the proposed action is useful.

## Independence without pretending to be isolated

AM is intended to outlast any one model, subscription, provider, storage system, or interface. A person ought to retain custody of their historical material and the commitments that govern future assistance.

Portability will still have costs: not every platform provides the same APIs, permissions, context, or interface. The project does not assume all providers can or should be interchangeable at the implementation level. It asks how to keep *the user's intent and provenance* portable even when tools differ.

An early research technique is to compare model reasoning **with and without carefully selected context**. More retrieved text may improve recall, but it can also supply a false premise with artificial confidence. Retrieval quality must be evaluated, not assumed.

## Candidate applications

**Personal context and research.** Revisit years of conversations and documents with traceable claims and correction history. Preserve the structure of an encounter or a decision, not just a summary that sounds convincing.

**Persistent objectives.** Resume technical work, correspondence, research, or administrative tasks after interruptions. Preserve goals and constraints without silently extending prior permissions.

**Evidence-aware finance.** Track a thesis, its sources, its challenges, and why a decision changed. Financial information is a possible research pilot, *not* implemented autonomous trading or wallet control.

**Technical and scientific work.** Connect hypotheses, experiments, counterexamples, failures, and verification evidence. Preserve unresolved anomalies instead of treating a successful rerun as an explanation.

These are possible directions. The value of each should be tested through actual use, not assumed from a diagram.

## Questions still open

How much context is enough? What should be omitted? Can a knowledge state be reconstructed using what was available historically, not just when an artifact was ingested? How should the system respond when a person and a model disagree about memory? How can it carry an objective forward without transforming persistence into autonomy? What independent evidence is necessary before reporting an irreversible effect?

AM remains research because these questions are not settled. The [public overview](README.md) summarizes the project; [STATUS.md](STATUS.md) separates demonstrated implementation from future work.
