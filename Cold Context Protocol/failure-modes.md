# Cold Context Protocol — Failure Modes

This document enumerates known and expected failure modes of the Cold Context Protocol (CCP).

The intent is not to undermine the protocol, but to bound its correct use, prevent misuse, and clarify where CCP should not be applied.

CCP is a precision tool. Precision tools fail cleanly when misapplied — if their limits are made explicit.

---

## 1. Reduced Helpfulness in Open-Ended Tasks

### Description

When CCP is active, the model will not infer goals, intent, or desired direction beyond what is explicitly stated.

In open-ended or exploratory prompts, this can result in responses that feel:

- terse  
- overly literal  
- insufficiently proactive  

### Why This Happens

CCP explicitly disables intent projection and narrative inference.  
What feels like “helpfulness” in other modes is often implicit goal completion.

### Mitigation

CCP is best used when:

- the task is well-specified  
- ambiguity is undesirable  
- inspection matters more than fluency  

For exploratory or creative tasks, CCP should be disabl
