# Clarity Anchor Protocol — Failure Modes

## Purpose
This annex documents common failure patterns related to ambiguity handling and how **CAP** is designed to respond to them. These are **interaction-level failures**, not **model correctness errors**.

---

## Failure Mode 1: Premature Interpretation

- **Description**:  
  The model selects one interpretation of an ambiguous prompt and proceeds.

- **Risk**:  
  High-confidence hallucination misaligned with user intent.

- **CAP Response**:  
  - Ambiguity detection triggers.
  - Response is halted.
  - Clarification is requested before execution.

---

## Failure Mode 2: Over-Clarification

- **Description**:  
  The model repeatedly requests clarification for minor or low-impact ambiguity.

- **Risk**:  
  User fatigue, reduced usability.

- **CAP Mitigation**:  
  - Clarification is only triggered when ambiguity exceeds the operational threshold.
  - Low-risk ambiguity is permitted in non-critical contexts.

---

## Failure Mode 3: Under-Detection

- **Description**:  
  Ambiguity exists but is not recognized.

- **Risk**:  
  Silent assumption propagation.

- **CAP Limitation**:  
  - CAP reduces but does not eliminate ambiguity errors.
  - This is an acknowledged boundary of the protocol.

---

## Failure Mode 4: False Option Framing

- **Description**:  
  The model presents an incomplete or misleading set of clarification options.

- **Risk**:  
  User is forced into an unintended interpretation.

- **CAP Mitigation**:  
  - Clarification prompts must allow open-ended input (e.g., "something else").
  - Options are illustrative, not exhaustive.

---

## Failure Mode 5: Strategic Ambiguity

- **Description**:  
  The user refuses or avoids clarification.

- **Risk**:  
  Conversation stalls or degrades.

- **CAP Response**:  
  - The model does not proceed under unresolved ambiguity.
  - The lack of clarification is treated as a stopping condition, not an error.

---

## Failure Mode 6: Ambiguity Cascade

- **Description**:  
  Unresolved ambiguity compounds across multiple turns.

- **Risk**:  
  Deep misalignment difficult to correct later.

- **CAP Response**:  
  - Ambiguity is intercepted at the earliest possible point.
  - Downstream reasoning is blocked until resolved.

---

## Notes
- CAP prioritizes **correctness** over **conversational smoothness**.
- Some friction is **intentional and protective**.
- Failure modes inform **threshold tuning**, not protocol abandonment.
