## Axioms & Invariants

### Purpose
This annex documents the foundational principles that **Structural Re-Location** relies upon. These axioms establish the assumptions, invariants, and operating constraints that make the protocol coherent, repeatable, and safe to apply in human–LLM interaction.

### Axioms

#### 1. Continuity is not guaranteed
Conversations, especially long-form interactions, naturally drift. Neither human memory nor model state guarantees persistent alignment of assumptions, claims, or implications. Structural Re-Location assumes drift occurs and explicitly addresses it.

#### 2. Structure precedes content
The conceptual tree—roots, trunk, branches, leaves—is the primary frame. Content (text, examples, illustrations) is secondary. Alignment on structure is sufficient to reduce hallucination even without enforcing factual correctness.

#### 3. Simultaneity matters
Drift arises when participants do not co-locate on the same conceptual structure at the same moment. The protocol assumes that simultaneous re-anchoring is required for meaningful structural alignment.

#### 4. Non-coercion preserves reliability
Protocol effectiveness does not require authority assertion, correction, or enforcement. Coercive mechanisms may destabilize human–model alignment or induce compliance without understanding.

#### 5. Observability enables accountability
Structural re-location steps must be explicit, observable, and understandable by both participants. Hidden operations cannot achieve the same drift-mitigation effect.

#### 6. Locality of effect
Re-anchoring operates at the interaction layer only. It does not assume global model updates, retraining, or memory reset. The structural frame exists temporarily to orient the conversation, not to overwrite prior knowledge.

#### 7. Minimal disruption
The protocol must interfere as little as possible with natural conversation flow. Optional mechanisms (Periodic Structural Check-In) should remain suggestive, not mandatory.

### Invariants

#### 1. Trunk Invariance
At any given point during a re-location, the main claim (trunk) is uniquely identified and agreed upon by both participants.

#### 2. Root Exposure
Active assumptions (roots) relevant to the trunk are fully surfaced and documented. Unstated or hidden roots are treated as potential drift sources until explicitly acknowledged.

#### 3. Branch Mapping
Major implications (branches) are explicitly traced from the trunk. Misaligned or abandoned branches are marked, preventing invisible divergence.

#### 4. Participant Co-Location
Both human and model are simultaneously positioned on the same trunk, roots, and branches before continuing the conversation.

#### 5. Operational Repeatability
Structural Re-Location can be performed repeatedly without altering the underlying model, content memory, or human reasoning beyond orientation.

#### 6. Structural Visibility
All active components of the conceptual tree (roots, trunk, branches, leaves) are accessible for review during the protocol execution.

### Notes
- These axioms and invariants are **explicit rules for interaction**, not model modifications.  
- Violation of any invariant is considered a structural failure; the protocol may be re-invoked to restore alignment.  
- The invariants reinforce the optional nature of the Periodic Structural Check-In: even when not invoked, the conceptual tree remains the operative frame for understanding conversation drift.
