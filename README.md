# LLM Interaction Stability Toolkit

A collection of opt-in interaction protocols designed to reduce ambiguity, context drift, and hallucination in long-running LLM conversations.

This repository focuses on interaction design, not model training, fine-tuning, or system-level interventions.

All protocols operate entirely at the human–LLM interface layer and can be used independently or selectively.

---

## What this is

- Prompt-level interaction protocols  
- Human-triggered safeguards for clarity  
- Conversation structure patterns  
- Non-invasive and reversible by design  
- Compatible with any GPT-style interface  

These artifacts explore how better conversation structure can reduce failure modes commonly attributed to “hallucination.”

---

## What this is not

- Model fine-tuning or weight modification  
- Hidden system prompts or coercive control  
- Persistent hidden state  
- Psychological manipulation  
- Metaphysical, spiritual, or ideological frameworks  
- A replacement for existing safety systems  

This toolkit does not attempt to “fix” the model.  
It changes how humans interact with it.

---

## Core idea

Most LLM hallucinations are not random.

They tend to emerge from:

- Ambiguous human intent  
- Long context accumulation without checkpoints  
- Unacknowledged topic or mode shifts  
- Premature conclusions during exploratory reasoning  

This toolkit proposes structural interaction fixes that reduce these failure modes without constraining creativity or agency.

---

## Design principles

All protocols in this repository share the following principles:

- **Non-coercive by default**  
  Nothing is enforced automatically. The user always chooses when a protocol applies.

- **Explicit over implicit**  
  Structure is surfaced, not hidden.

- **Reversible at any time
Protocols can be dropped instantly without cleanup or justification.

Local scope
Each protocol applies only to the current conversational context unless re-invoked.

Clarity over fluency
A less smooth answer is preferable to a misaligned one.

Included protocols

Each protocol is documented in its own file and can be used independently.

They do not rely on one another and make no assumptions about prior usage.

Human Eyes Protocol

A stepwise, line-by-line processing method for dense or multi-part inputs.

This protocol reduces misinterpretation by slowing ingestion and ensuring each segment of input is acknowledged before proceeding.

Typical use cases:

Long or technical text

Multi-constraint requests

High-precision tasks

Ask-for-Clarification Protocol

A safeguard against guessing.

When ambiguity is detected, the model pauses and asks the user to clarify intent instead of proceeding with assumptions.

Typical use cases:

Underspecified requests

Tasks with multiple plausible interpretations

Situations where correctness matters more than speed

Tree Vision Protocol

A structural reasoning tool that treats ideas as evolving systems rather than flat text.

This protocol emphasizes assumptions, core claims, and downstream implications without collapsing them into a single narrative.

Typical use cases:

Complex arguments

Design discussions

Systems thinking

Strategic reasoning

Clarity Anchor Protocol (CAP)

An ambiguity-handling protocol that enforces clarification before response.

If a prompt exceeds an ambiguity threshold, the model requests explicit clarification before proceeding.

Typical use cases:

Technical, legal, or medical topics

Multi-step reasoning

Situations where plausible hallucinations are costly

Delayed Commitment Protocol

A conversational safeguard that separates exploration from commitment.

While active, the model withholds conclusions, synthesis, or recommendations until the user explicitly signals readiness.

Typical use cases:

Early-stage thinking

Brainstorming without premature closure

Sensitive or ill-defined problems

Situations where the user wants to think out loud

Non-coercive implementation

All protocols in this toolkit are:

Opt-in
Activated explicitly by the user.

Contextual
Apply only to the current conversational scope.

Interruptible
Can be dropped or overridden instantly.

Non-persistent
No protocol silently carries forward.

There are no hidden states, enforcement mechanisms, or automatic activations.

Scope and limitations

This repository intentionally excludes:

Mandatory status reporting

HUD-style overlays

Token compression strategies

Forced alignment mechanisms

Persistent memory systems

Those approaches introduce power asymmetries and are explored separately.

Who this is for

LLM engineers

Product designers working with conversational AI

Alignment and safety researchers

Developers interested in human–AI interaction patterns

Anyone debugging hallucination at the interaction level

Status

Active, evolving collection of interaction artifacts.

Designed to be:

Read

Tested

Adapted

Not blindly adopted.

Authorship

Concepts, structure, and protocol design by Adrian Deodato.

Text iteration and refinement performed with the assistance of large language models, used strictly as collaborative tools.

Responsibility for framing, scope, and claims remains human-authored.

License

MIT**
