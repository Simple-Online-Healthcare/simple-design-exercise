# Design Exercise: Personalised “Patients Like Me” Outcomes

## Context
We’re exploring a potential feature to help patients understand real-world treatment outcomes from people similar to them.

A typical question might be:

> **“Do you have results from patients like me?”**

Assume we hold a range of internal information such as anonymised outcome data, knowledge base content and clinical guidance. AI models could be used to help generate personalised responses.

This is a **theoretical design exercise** — you don’t need to build anything or have deep AI experience.

---

## The task
Design an approach for a tool that can generate a personalised response to a patient asking:

> **“Show me patients like me and what results they saw.”**

Assume:
- the response must be trustworthy and suitable for a healthcare setting
- AI is available as a capability to help retrieve, synthesise and personalise information
- this is pre-treatment decision support (not diagnosis or prescribing)

You can make reasonable assumptions — just state them.

---

## We’ll explore together
We’re interested in how you think about:
- clarifying requirements and defining the problem
- what a good and trustworthy response looks like
- how AI might be used within the experience
- risks and failure modes
- how you would measure success

There is no single correct answer — treat this as a collaborative design discussion.

---

## Format
45–60 minute working session.  
No preparation needed.

---

## Conceptual tool map (for discussion)

This is one possible shape. Please feel free to ignore or redesign it.

```mermaid
flowchart TD
  U[Patient question]

  U --> D[Available data sources]
  U --> AI[AI capabilities]

  D --> S[Response generation]
  AI --> S

  S --> R[Patient-facing answer]

