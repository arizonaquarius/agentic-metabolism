# Agentic Metabolism

Agentic Metabolism is an experimental personal-agent architecture focused on
bounded authority, durable state, auditability, and safe interaction with
external tools and untrusted workloads.

The project is currently in early development.

Its central research question is straightforward:

> How can a durable software agent be given meaningful capabilities without
> giving those capabilities unlimited or ambiguous authority?

Rather than beginning with a large collection of agent features, Agentic
Metabolism is being developed from the authority and execution boundary outward.

---

## Design goals

The project is exploring an agent architecture in which:

- capabilities are explicitly granted rather than assumed
- authority can be scoped to a particular task or execution lifetime
- untrusted workloads execute inside constrained environments
- protected state is separated from workload-accessible state
- consequential actions are attributable and auditable
- resource use can be bounded
- failures should degrade safely rather than silently expanding authority
- future subsystems can be added without weakening the underlying authority model

The goal is not to build an unrestricted autonomous system.

The goal is to understand what minimum mechanisms are required for a useful
agent to operate within enforceable boundaries.

---

## Current research focus

The current phase of development is focused on a minimal agent kernel and its
security properties.

Work to date has concentrated on:

- authority and capability boundaries
- workload lifecycle semantics
- separation between privileged kernel state and workload state
- explicit interfaces between trusted and untrusted components
- audit and provenance requirements
- failure and termination behavior
- resource and permission constraints
- containment requirements for untrusted code

The architecture is intentionally being developed before broadening the
agent's operational capabilities.

---

## Adversarial validation

A major upcoming phase of the project is adversarial validation of the kernel's
security assumptions.

This testing is defensive.

Untrusted or adversarial workloads may be used inside controlled test
environments to determine whether they can violate declared system invariants,
including attempts to:

- access state outside their assigned execution compartment
- obtain credentials or protected information
- modify their own permissions or authority
- persist beyond their authorized lifetime
- communicate outside permitted network boundaries
- consume resources beyond assigned limits
- interfere with audit evidence or execution records

The objective is not merely to observe that a workload behaved correctly.

The objective is to produce evidence showing where a prohibited action was
stopped and which enforcement boundary was responsible.

For example:

    workload request
        -> authority decision
        -> enforcement boundary
        -> result
        -> audit record

This distinction matters because cooperative model behavior is not considered a
substitute for structural containment.

---

## Security philosophy

Hostile code is not part of normal Agentic Metabolism operation.

Adversarial execution exists as test equipment for validating the system that
will run ordinary workloads.

The project assumes that application-level instructions can fail, untrusted
inputs can be deceptive, and individual components can behave incorrectly.
Important security properties should therefore be enforced by architecture and
execution boundaries rather than by model obedience alone.

Security claims are treated as hypotheses until they can be tested.

---

## Scope and authorization

Security testing conducted as part of Agentic Metabolism is limited to systems,
software, accounts, and environments owned by or explicitly authorized for use
by the project operator.

The project is not intended for unauthorized access, third-party exploitation,
credential theft, persistence on external systems, or testing against systems
without permission.

Where possible, adversarial tests use synthetic credentials, disposable state,
test resources, and controlled network targets.

If project research reveals a vulnerability in third-party software, the intent
is to handle it through appropriate responsible-disclosure channels rather than
public exploitation.

---

## Current status

**Early research / pre-release**

The kernel and its security model are still under active development.

Current work is moving from architectural definition toward reproducible
security validation. Some security properties have been specified but should
not yet be interpreted as proven.

The project is not currently intended for production deployment.

---

## Why advanced cybersecurity model access is relevant

Agentic Metabolism is approaching a stage where meaningful defensive validation
requires reasoning about how untrusted code could deliberately violate sandbox,
authority, persistence, resource, and data-access boundaries.

More capable cybersecurity models would be used to:

- develop defensive threat models
- design controlled adversarial test cases
- identify weaknesses in containment assumptions
- analyze unexpected sandbox behavior
- validate mitigations and patches
- improve the project's security test coverage

The intended use is defensive validation of an owned research environment.

Advanced offensive capability is not required for the agent's ordinary
operation.

---

## Repository scope

This repository currently serves as the public description of the project.

Implementation, detailed security-test artifacts, machine-specific
configuration, credentials, and sensitive research material are intentionally
not published here.

Additional architecture and security documentation may be added as the project
matures and material can be published without weakening the systems being
tested.

---

## Project principles

Agentic Metabolism is being developed around a few persistent ideas:

**Authority should be explicit.**

A component should not gain access merely because it can reach another
component.

**Containment should survive non-cooperation.**

A security boundary should not depend on an agent or workload choosing to obey
it.

**Consequential actions should leave evidence.**

Important state changes should be attributable and reconstructable.

**Complexity should be earned.**

New capabilities should be added only when the underlying boundaries remain
understandable and testable.

**Security claims should be testable.**

"The system appears safe" is weaker than a specific invariant that can be
deliberately challenged.

---

## License

A project license has not yet been selected.
