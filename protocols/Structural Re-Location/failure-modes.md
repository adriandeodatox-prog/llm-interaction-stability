## Failure Modes

### Purpose
This annex documents the structural drift patterns and failure scenarios that **Structural Re-Location** is designed to detect and mitigate. Understanding these modes helps in both designing interactions and evaluating protocol effectiveness.

### Common Failure Modes

#### 1. Trunk Drift
- **Description:** The main claim (trunk) slowly shifts during conversation without explicit acknowledgment.  
- **Effect:** Participants believe they are aligned on the core topic, but discussions diverge in subtle ways.  
- **Detection:** Re-location identifies misalignment between assumed and actual trunk.

#### 2. Root Creep
- **Description:** Assumptions (roots) gradually accumulate or change without surfacing.  
- **Effect:** Implicit assumptions influence reasoning, leading to misinterpretation or unseen conflicts.  
- **Detection:** Structural Re-Location surfaces active roots to expose hidden drift.

#### 3. Branch Hopping
- **Description:** The conversation jumps between implications (branches) unpredictably, skipping intermediate reasoning.  
- **Effect:** Accumulated narrative fog; human or model may misattribute conclusions or claim coherence that is absent.  
- **Detection:** Re-location maps branches explicitly, marking abandoned or misaligned ones.

#### 4. Leaf Noise
- **Description:** Minor details, examples, or tangents (leaves) accumulate and distract from the trunk.  
- **Effect:** Cognitive overload, misinterpretation, and potential hallucination.  
- **Detection:** Leaves are tracked as peripheral; irrelevant leaves are marked or collapsed.

#### 5. Implicit Assumption Masking
- **Description:** Hidden or unstated assumptions remain unchallenged.  
- **Effect:** Apparent agreement masks misalignment, leading to false confidence in conclusions.  
- **Detection:** Roots are surfaced; any hidden assumptions are explicitly questioned or noted.

#### 6. Human Drift
- **Description:** The human participant loses track of the conceptual tree, making implicit or forgotten assumptions.  
- **Effect:** Miscommunication, unnoticed drift, and higher susceptibility to model hallucination.  
- **Detection:** Optional: Periodic Structural Check-In prompts realignment without coercion.

#### 7. Model Drift
- **Description:** The LLM gradually changes focus, prioritizes different branches, or misidentifies the trunk.  
- **Effect:** Misalignment with human reasoning, potential hallucination.  
- **Detection:** Re-location enforces explicit trunk identification and branch mapping.

### Notes
- Structural Re-Location is explicitly designed to **intervene on these failure modes** without correcting content or enforcing “truth.”  
- Optional mechanisms, like the Periodic Structural Check-In, allow subtle realignment before drift propagates.  
- Consistent application of the protocol **prevents compounding drift**, stabilizing the shared conceptual tree across long interactions.

