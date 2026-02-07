# Failure Modes
## Delayed Commitment Protocol (DCP)

This document outlines failure patterns DCP is designed to prevent, as well as edge cases where misuse may reduce effectiveness.

---

## Addressed Failure Modes

### 1. Premature Synthesis

The model converges on a conclusion while assumptions are still unstable.

DCP blocks this by withholding synthesis until explicitly requested.

---

### 2. Narrative Lock-In

Early conclusions bias later reasoning, making correction difficult.

Delayed commitment keeps narrative space open.

---

### 3. False Agreement

The appearance of alignment caused by early closure rather than actual shared understanding.

DCP preserves multiple interpretations until alignment is explicit.

---

### 4. Recommendation Momentum

Models default to “helpful advice” even when the human is still exploring.

DCP removes unsolicited recommendations.

---

## Edge Case Failure Modes

### Over-Deferral

If the human never signals commitment, conversations may remain exploratory indefinitely.

This is not a protocol failure, but a consequence of its design.

---

### Misinterpreted Signals

Ambiguous phrases may be mistaken for commitment signals.

Mitigation: treat commitment triggers conservatively and request confirmation when unclear.

---

### Inappropriate Use

Applying DCP to trivial or time-critical queries may feel obstructive.

The protocol is opt-in and context-sensitive by design.

---

## Non-Failures

The following are not considered failures under DCP:

- Long exploratory exchanges  
- Repeated clarification without conclusion  
- Abandoned conversations without synthesis  

These outcomes reflect correct adherence to delayed commitment.
