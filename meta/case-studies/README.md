# Case Studies

This folder contains illustrative case studies demonstrating how the protocols in this repository behave in realistic interaction scenarios.

These case studies are **not benchmarks, experiments, or evaluations**.
They are narrative walkthroughs intended to make protocol behavior concrete and observable.

Each case study focuses on:

- a specific interaction context
- a common failure mode (e.g. ambiguity, drift, premature closure)
- how a single protocol changes the interaction dynamics

The goal is clarity, not proof.

## Scope

Case studies in this folder:

- are protocol-specific
- do not rely on one another
- do not claim general performance improvements
- do not assume any model internals or training changes

They illustrate interaction patterns only.

## Structure

Each protocol has its own case study file following a shared structure:

- Scenario
- Without the protocol
- With the protocol applied
- Observed interaction effect

No metrics, scoring, or quantitative claims are used.

## Intent

These case studies exist to help readers:

- understand when a protocol is useful
- recognize the failure modes it targets
- decide whether it fits their own interaction needs

They are examples, not prescriptions.
