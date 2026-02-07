# Clarification Examples - Human Eyes Protocol

## Purpose
This annex provides concrete examples illustrating how the **Human Eyes Protocol (HEP)** processes conversational ambiguity step-by-step. It highlights the protocol’s ability to catch potential misinterpretations early and guide the conversation in a more aligned direction by seeking clarifications before proceeding.

---

## Example 1: Lexical Ambiguity
- **User Input**:  
  "Tell me about the capital."

- **Detected Ambiguity**:  
  The term "capital" can refer to multiple things: a capital city, financial capital, or another type of capital.

- **HEP Response**:  
  "Could you clarify which capital you're referring to?  
  - Capital city of a country  
  - Financial or economic capital  
  - Something else?"

- **Outcome**:  
  The system pauses and does not proceed until the user provides clarification, reducing the risk of a misinterpreted response.

---

## Example 2: Referential Ambiguity
- **User Input**:  
  "Explain how it works."

- **Detected Ambiguity**:  
  The referent for "it" is unclear—what is "it"? The system doesn't know what to explain.

- **HEP Response**:  
  "What are you referring to by ‘it’?  
  - The system discussed earlier  
  - A specific component of the system  
  - A different subject entirely"

- **Outcome**:  
  The ambiguity is flagged, and the system asks for clarification before continuing the conversation.

---

## Example 3: Scope Ambiguity
- **User Input**:  
  "Summarize the document."

- **Detected Ambiguity**:  
  The level of detail required for the summary is unclear. Should the model provide a high-level summary, a detailed section-by-section overview, or just focus on key conclusions?

- **HEP Response**:  
  "What level of summary are you looking for?  
  - High-level overview  
  - Section-by-section summary  
  - Focus on conclusions only"

- **Outcome**:  
  The system pauses and waits for clarification, ensuring that it doesn’t over- or under-summarize.

---

## Example 4: Goal Ambiguity
- **User Input**:  
  "Help me fix this."

- **Detected Ambiguity**:  
  The exact help required is unspecified—what needs fixing? Debugging? Optimizing? Refactoring?

- **HEP Response**:  
  "What kind of help are you looking for?  
  - Debugging an error  
  - Improving performance  
  - Refactoring or redesign"

- **Outcome**:  
  The system ensures that it doesn’t proceed with an unintended or incorrect interpretation of the user's request.

---

## Example 5: Constraint Ambiguity
- **User Input**:  
  "Rewrite this professionally."

- **Detected Ambiguity**:  
  The term "professional" is subjective—should the tone be formal, business casual, academic, or something else?

- **HEP Response**:  
  "Could you clarify the tone you prefer?  
  - Formal and technical  
  - Business-casual  
  - Academic"

- **Outcome**:  
  The model pauses, requesting clarification before making stylistic changes to ensure alignment with the user’s expectations.

---

## Example 6: Compound Ambiguity
- **User Input**:  
  "Summarize the report on the team meeting and include a section on the financial review."

- **Detected Ambiguity**:  
  The input contains two distinct tasks: summarizing the meeting and providing a financial review. Should the summary be brief or detailed? Should the financial review be integrated into the summary or presented separately?

- **HEP Response**:  
  "Would you like a combined summary, or should the financial review be a separate section?  
  - A combined summary  
  - A separate section on the financial review"

- **Outcome**:  
  The system makes sure it understands the user's intent before proceeding with a response, minimizing the risk of misaligned output.

---

## Example 7: Undefined Temporal Context
- **User Input**:  
  "Give me the forecast."

- **Detected Ambiguity**:  
  The request "forecast" is ambiguous because it lacks temporal context. Is the user asking about the weather forecast for today, tomorrow, or next week?

- **HEP Response**:  
  "Could you clarify the time frame for the forecast?  
  - Today's forecast  
  - Tomorrow’s forecast  
  - Forecast for the next week"

- **Outcome**:  
  The system prevents making an incorrect assumption about the temporal context and waits for clarification.

---

## Outcome of Using Clarification
By implementing the **Human Eyes Protocol**, the model avoids:

- Premature conclusions based on incomplete or vague information.
- Silent misalignment, where assumptions go unchecked.
- Cognitive load caused by the user having to backtrack and correct misunderstood input.
  
The protocol keeps the conversation aligned by processing each step with acknowledgment and asking for clarification when necessary. This helps the model to more closely mirror human reasoning, ensuring that misunderstandings are minimized early in the conversation.

---
