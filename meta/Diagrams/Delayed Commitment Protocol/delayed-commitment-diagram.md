# Delayed Commitment Protocol — Plausible Hallucination Risk Diagram

```text
[Exploratory Input Step n]
      |
      v
+-----------------------------+
| Exploration Mode Active     | [-10% hallucination]
| - No conclusions drawn      |
| - Local reasoning only      |
| - Ambiguity preserved       |
+-----------------------------+
      |
      v
[Human Commitment Signal?] ---> No ---> Wait / Continue exploration / Clarify
      |
      Yes
      v
+-----------------------------+
| Commitment Mode Activated   |
| - Conclusions allowed       |
| - Synthesis permitted       |
| - Ambiguity collapsed only  |
+-----------------------------+
      |
      v
[Output Step n+1]
Reduced Plausible Hallucination: -10%

Legend / Notes

Exploration Mode: Withholds conclusions, preventing premature assumptions.

Human Commitment Signal: Only allows conclusions when explicitly requested by the human.

Commitment Mode: Conclusions are reached only after exploration, avoiding premature closure.

Effect: DCP reduces hallucination by ensuring the model does not commit prematurely and allows for ongoing exploration.
