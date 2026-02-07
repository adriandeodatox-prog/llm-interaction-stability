# Cold Context Protocol — Plausible Hallucination Risk Diagram
[Input Step n]
      |
      v
+---------------------------+
| CCP Context Isolation     | [-30% hallucination]
| - Only current input valid|
| - All other context sealed|
+---------------------------+
      |
      v
[Jar Activation Required?] ---> No ---> Proceed without sealed context / Request clarification
      |
      Yes
      v
+---------------------------+
| Explicit Jar Access       |
| - Identity, History, etc. |
| - Bounded scope & duration|
+---------------------------+
      |
      v
[Deterministic Interaction]
- Literal parsing only
- Local reasoning only
- No implicit inference
      |
      v
[Optional Orientation?] ---> Non-binding suggestion for continuity
      |
      v
+---------------------------+
| Output Step n+1           |
+---------------------------+
Reduced Plausible Hallucination: -30%
