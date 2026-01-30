# LLM Interaction Stability Toolkit

A collection of opt-in interaction protocols designed to reduce ambiguity,
drift, and hallucination in long-running LLM conversations.

This repository focuses on **interaction design**, not model training or fine-tuning.

## What this is

- Prompt-level protocols
- Conversation structure patterns
- Opt-in safeguards for clarity and alignment
- Zero-invasiveness: no hidden state, no coercion

## What this is not

- Model fine-tuning
- Psychological manipulation
- Metaphysical or spiritual claims
- A replacement for safety systems

## Core idea

Most hallucinations are not "random".
They emerge from:
- Ambiguous human intent
- Long context drift
- Unacknowledged mode shifts
- Overload without checkpoints

This toolkit proposes **structural interaction fixes** instead of model changes.

## Initial protocols

- Human Eyes (stepwise reading)
- Ask-for-Clarification Protocol (ambiguity choke)
- Drift Control (anchors and re-alignment)
- Tree Vision (structural summarization)

Each protocol is:
- Optional
- Human-triggered
- Reversible
