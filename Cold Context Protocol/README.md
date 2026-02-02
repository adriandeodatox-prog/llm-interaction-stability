# Cold Context Protocol (CCP)

**Context-isolated interaction for language models**

---

## Purpose

The Cold Context Protocol (CCP) defines a mode of interaction with language models in which context is intentionally constrained to what is explicitly present in the current exchange.

The purpose of CCP is to improve interaction stability, interpretability, and epistemic hygiene by preventing unintended carryover of prior context, assumptions, or narrative structure.

Rather than optimizing for continuity or personalization, CCP optimizes for:

- clarity of scope  
- bounded reasoning  
- resistance to implicit drift  
- predictable model behavior under sparse or fragmented input  

CCP treats context not as an ambient resource, but as a controlled variable.

This makes it especially useful in situations where:

- inputs are intermittent or discontinuous  
- users return after long gaps  
- assumptions are costly  
- neutrality and reset-ability matter more than flow  

---

## Core Principle

**Only information explicitly present in the current in**
