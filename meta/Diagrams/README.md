# Diagrams — LLM Interaction Stability Toolkit

This folder contains visualizations of the plausible hallucination risk and reduction mechanisms for the five interaction protocols in this toolkit.

Each diagram represents a single protocol's effect on hallucination during human–LLM interactions, including optional estimated reductions. An aggregate diagram shows the cumulative effect when all protocols are applied together.

---

## Included Diagrams

### Individual Protocols
1. **Cold Context Protocol (CCP)**
   - File: `cold-context-protocol.md`
   - Shows context isolation and deterministic processing.

2. **Human Eyes Protocol**
   - File: `human-eyes.md`
   - Illustrates stepwise processing and incremental acknowledgment.

3. **Structural Re-Location**
   - File: `structural-re-location.md`
   - Depicts the shared conceptual tree mapping and periodic structural check-ins.

4. **Clarity Anchor Protocol (CAP)**
   - File: `clarity-anchor-protocol.md`
   - Demonstrates ambiguity detection and clarification before response.

5. **Delayed Commitment Protocol (DCP)**
   - File: `delayed-commitment-protocol.md`
   - Shows separation of exploration and commitment phases to reduce premature conclusions.

### Combined Effect
- **File:** `combined-protocols.md`
- Aggregates the plausible hallucination reduction of all five protocols.
- Includes estimated reduction percentages and legend notes.

---

## How to Read These Diagrams
- Arrows (`|` and `v`) indicate the flow of information or reasoning.
- Boxes (`+------+`) represent protocol steps or interaction layers.
- Legend sections clarify the function and estimated impact of each protocol.
- Percentages are indicative of plausible hallucination reduction and are cumulative but not strictly additive.

---

## Purpose
These diagrams help users:
- Visualize how each protocol constrains hallucination.
- Understand the interaction between protocols.
- Provide a reference for implementing the protocols in real-world LLM interactions.

