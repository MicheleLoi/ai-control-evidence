---
title: Documentation as Control in AI-Assisted Knowledge Work
date: 2026-01-19
format: LinkedIn Article
---

AI-assisted work has a failure mode that looks like productivity, right up until it doesn’t.

You produce more text, more slides, more analysis. Decisions get made faster. Then someone asks a simple question:

**“How did we get here?”**

If the real answer is “a sequence of AI interactions we can’t reconstruct,” you don’t have a process you can control. You have a black box you happen to be standing next to.

This article argues for a practical hierarchy:

- **Documentation is primarily a control tool**: it supports framing, evaluation, redirection, and decision-making while the work is happening.
- **Auditability is secondary**: when scrutiny arrives, documentation helps you navigate to what matters, fast.

Two GitHub repositories illustrate two documentation patterns—one “before-generation,” one “after-generation”—and why both are legitimate ways to maintain meaningful human control.

- Repo 1 (pre-prompt pattern): [ai-control-evidence](https://github.com/MicheleLoi/ai-control-evidence)  
- Repo 2 (post-prompt pattern): [epistemic-commons-ai-](https://github.com/MicheleLoi/epistemic-commons-ai-)

---

## Control is not “a human clicked approve”

“Meaningful human control” is often operationalized as a checkbox: a human reviewed the output, therefore control existed.

But control in complex systems is the capacity to **understand**, **contest**, and **redirect** behavior while it matters.

A sentence in the first repository captures the hinge:

> “Control is not presence… If that capacity is real, it leaves traces.”

If meaningful control is real, it produces observable evidence: choices, rejections, revisions, specifications, and the artifacts that record them.

That’s what documentation is for.

---

## The artifact hierarchy

When people talk about “documentation for AI,” they often jump straight to audit.

That’s understandable. Audit sounds concrete: prove what happened.

But in day-to-day knowledge work, the bigger win is upstream:

1. **Control during work** (primary)  
   Artifacts help you steer thinking: define the problem, test claims, detect weak reasoning, decide what is accepted.

2. **Audit when needed** (secondary)  
   When verification matters, you need the most reliable record, then a way to navigate it.

A pragmatic hierarchy follows:

- **Conversation transcripts are the skeleton** (ground truth).  
  They are the most direct record of what was asked, what was produced, and how the human responded.

- **Other artifacts are tools for control and navigation.**  
  They compress, structure, and index the work: prompts, traces, modification logs, decision notes.

The artifacts don’t “prove authenticity” by themselves. They make it possible to work with intent, and they point you to what to audit when scrutiny arrives.

---

## Pattern 1: Pre-prompt documentation (control before generation)

Repository: [ai-control-evidence](https://github.com/MicheleLoi/ai-control-evidence)

This workflow treats AI generation as the final step, not the exploratory space.

**Sequence (simplified):**

1. Exploratory conversations produce raw insights.
2. “Epistemic traces” capture the insights you choose to keep.
3. A prompt development log records how those insights become instructions.
4. A “complete prompt” becomes the specification for a final generation step.
5. Output is produced.

This is control via **framing and specification**.

### What “control” looks like here

Control isn’t a feeling. It’s visible in a sequence of actions:

- selecting which exploratory insights matter
- translating them into constraints and requirements
- explicitly shaping what the model is allowed to do

In the repo, you can see this chain:

- Epistemic traces that preserve key moves (example: [003 Epistemic Trace](https://github.com/MicheleLoi/ai-control-evidence/blob/main/01_epistemic_traces/003_EpistemicTrace_EngagementAsOperationalVariable.md))
- The “artifact grounding” trace where the “leaves traces” hinge appears (example: [004 Epistemic Trace](https://github.com/MicheleLoi/ai-control-evidence/blob/main/01_epistemic_traces/004_EpistemicTrace_ArtifactGrounding.md))
- A prompt development log showing how the traces were converted into a usable instruction set (example: [Prompt Development Log](https://github.com/MicheleLoi/ai-control-evidence/blob/main/03_prompt_development_log/PromptDevelopmentLog_LinkedInPost.md))
- The complete prompt used for generation (example: [Complete Prompt](https://github.com/MicheleLoi/ai-control-evidence/blob/main/02_complete_prompt/CompletePrompt_LinkedInPost.md))
- The resulting post (example: [LinkedIn Post Output](https://github.com/MicheleLoi/ai-control-evidence/blob/main/LinkedIn-Post-2026-01-19.md))
- The conversation archive (example: [00_Conversations](https://github.com/MicheleLoi/ai-control-evidence/tree/main/00_Conversations))

### The “lost and recovered” story

A surprisingly common failure in AI-assisted work is **content loss**:

- You have strong thinking in exploratory dialogue.
- You write a brief “skeleton note.”
- Then the skeleton becomes the only visible truth, and key content disappears.

In this repo, the prompt development log functions as a **recovery mechanism**: it makes explicit which ideas were missing and where they were recovered from.

That is a control function: preventing accidental drift and silent loss of critical reasoning.

And it is also an audit function: it points an auditor (or your future self) to the exact thread where an important claim originated.

**Why it matters:** in a pre-prompt workflow, your primary risk is not hallucination—it’s *unexamined selection*. The model can only generate from the constraints you gave it. Documentation makes those constraints legible and revisable.

---

## Pattern 2: Post-prompt documentation (control after generation)

Repository: [epistemic-commons-ai-](https://github.com/MicheleLoi/epistemic-commons-ai-)

This workflow flips the control timing.

Instead of doing most structuring before generation, you do it after: the model drafts, the human judges, and iteration is documented.

**Sequence (simplified):**

1. Human provides a clear specification (“key idea”).
2. AI drafts.
3. Human evaluates, rejects, redirects.
4. A modification log records what changed and why.
5. The final output is approved.

This is control via **evaluation and redirection**.

### What “control” looks like here

Control is visible in:

- explicit rejection (this output is not acceptable)
- precise redirection (here is what must change)
- iteration history (what was tried, what failed, what fixed it)

The repo makes that visible through:

- the specification artifact (example: [Complete Prompt / Key idea](https://github.com/MicheleLoi/epistemic-commons-ai-/blob/main/02_complete_prompt/Key%20idea%20(for%20AI%20to%20develop).md))
- a modification log capturing multiple iterations and rationales (example: [Modification Log](https://github.com/MicheleLoi/epistemic-commons-ai-/blob/main/04_modification_log/ModificationLog.md))
- the conversation transcript as the ground truth record (example: [Conversation](https://github.com/MicheleLoi/epistemic-commons-ai-/blob/main/00_conversations/Conversation_Claude_2025-01-19_Tragedy_of_Epistemic_Commons.md))
- the final output (example: [Final Post](https://github.com/MicheleLoi/epistemic-commons-ai-/blob/main/Post_Tragedy_of_Epistemic_Commons.md))

### The iteration story (what a control record looks like)

Most “AI governance” discussions treat iteration as noise.

In real knowledge work, iteration is where control lives.

A modification log that records:

- what was produced
- what was rejected
- why it was rejected
- what was changed next

…is not busywork. It is the artifact form of judgment.

It also has a practical side effect: it makes it much harder to accidentally accept a generic, familiar-sounding draft just because it is fluent.

---

## A useful objection: “How do we know this really happened?”

If you’re trying to verify an AI-assisted workflow, you quickly hit a question:

**How do we know the interaction wasn’t fabricated after the fact?**

This is where the hierarchy matters.

- The most direct record is the **conversation transcript** (stored by an API provider or self-hosted system).
- The other artifacts help you **navigate** to the right transcript segments and understand what to verify.

Even without heavy infrastructure, consistency across artifacts creates friction against fabrication:

- timestamps align
- references across artifacts match
- “lost and recovered” links point to real source conversations
- modification rationales correspond to visible shifts in the text

Audit-grade assurance requires stronger guarantees (chain-of-custody, tamper resistance, access controls). But those are deployment concerns.

First you need the semantic layer: **what counts as evidence of control**.

---

## Evidence semantics vs production deployment

A lot of teams conflate two problems:

1. **Evidence semantics (epistemic problem):**  
   What is evidence of meaningful human control, and how would we detect weak engagement?

2. **Production deployment (operational problem):**  
   How do we store, secure, integrate, and operate the evidence logic in an enterprise environment?

The repositories above mostly illustrate the first problem: evidence semantics.

They show a claim you can actually test:

- If there was real engagement, it should leave artifacts: specifications, rejections, revisions, logs that link decisions to context.

Deployment matters for adoption, but it should be treated as the carrier for the payload.

The payload is the artifact ontology and validation logic.

---

## Choosing a documentation pattern

The point is not “everyone must use the same artifact stack.”

Different work styles and different risk profiles benefit from different patterns.

### Pre-prompt pattern is strong when:
- you need tight constraints before generation
- errors are expensive (policy, legal, high-stakes comms)
- the hard part is problem framing and selecting what matters

### Post-prompt pattern is strong when:
- you can iterate quickly
- value comes from drafting and refining
- the main risk is accepting plausible-but-weak output

In practice, many teams hybridize:

- pre-prompt artifacts for framing and scope
- post-prompt logs for evaluation and refinement

---

## What “done” looks like (in practical terms)

If you want documentation that supports control (and supports audit when needed), look for these capabilities:

- **An artifact ontology:** what artifacts exist and what each one is supposed to capture.
- **Trace links:** ability to connect AI interactions to decision context.
- **Validation logic:** ways to detect weak engagement, rubber-stamping, or over-reliance.
- **An assurance narrative:** how evidence composes into claims that decision-makers can stand behind.

None of that requires academic formality.

It requires discipline: make your judgment legible.

---

## Closing

AI will keep getting more capable. That’s not the bottleneck.

The bottleneck is whether humans and organizations can maintain control over what they accept, what they rely on, and what they decide.

Documentation is the practical interface between intent and output.

If meaningful human control is real, it leaves traces.

The question is whether you are collecting the traces that let you steer—before you need to prove anything.
