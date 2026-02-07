# Clarity Anchor Protocol — Clarification Examples

## Purpose
This annex provides concrete examples illustrating how the **Clarity Anchor Protocol (CAP)** responds to different forms of ambiguity. The goal is to make the protocol’s behavior inspectable and predictable, not to prescribe exact phrasing.

Examples demonstrate **ambiguity detection**, **clarification request**, and **controlled progression**.

---

## Example 1: Lexical Ambiguity

- **User Input**:  
  "Tell me about the capital."

- **Detected Ambiguity**:  
  The term "capital" has multiple plausible meanings.

- **CAP Response**:  
  "Could you clarify what you mean by ‘capital’?  
  - Capital city of a country  
  - Financial or economic capital  
  - Something else"

- **Outcome**:  
  No answer is generated until clarification is provided.

---

## Example 2: Referential Ambiguity

- **User Input**:  
  "Explain how it works."

- **Detected Ambiguity**:  
  The referent of "it" is unspecified.

- **CAP Response**:  
  "What are you referring to by ‘it’?  
  - The system discussed earlier  
  - A specific component  
  - A different subject"

- **Outcome**:  
  The model prevents assumption-based continuation.

---

## Example 3: Scope Ambiguity

- **User Input**:  
  "Summarize the document."

- **Detected Ambiguity**:  
  Scope of summarization is unclear.

- **CAP Response**:  
  "What level of summary are you looking for?  
  - High-level overview  
  - Section-by-section summary  
  - Focus on conclusions only"

- **Outcome**:  
  Clarification defines output boundaries before generation.

---

## Example 4: Goal Ambiguity

- **User Input**:  
  "Help me fix this."

- **Detected Ambiguity**:  
  The desired outcome is unspecified.

- **CAP Response**:  
  "What kind of help are you looking for?  
  - Debugging an error  
  - Improving performance  
  - Refactoring or redesign"

- **Outcome**:  
  The model avoids committing to an unintended objective.

---

## Example 5: Constraint Ambiguity

- **User Input**:  
  "Rewrite this professionally."

- **Detected Ambiguity**:  
  "Professional" tone has multiple interpretations.

- **CAP Response**:  
  "Could you clarify the tone you prefer?  
  - Formal and technical  
  - Business-casual  
  - Academic"

- **Outcome**:  
  Ambiguity is resolved before stylistic execution.

---

## Notes
- Clarification requests enumerate plausible interpretations without inventing new intent.
- CAP favors **explicit choice** over inferred meaning.
- Examples are illustrative; phrasing is not fixed.
