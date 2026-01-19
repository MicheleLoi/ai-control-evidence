# AI Control Evidence

This repository contains the artifact chains behind two related publications on meaningful human control in AI systems:

1. **LinkedIn Post** (`LinkedIn-Post-2026-01-19.md`) — A short piece arguing that engagement is observable behavior that produces artifacts. Built using the **specification-first** pattern.

2. **LinkedIn Article** (`LinkedIn-Article-2026-01-21.md`) — A longer piece comparing two documentation patterns for maintaining meaningful human control. Built using **both** patterns: specification work upfront, then iteration and refinement.

---

## Two Documentation Patterns

The Article describes two workflows for maintaining meaningful human control. This repo and a companion repo provide examples.

### Specification-first

Control is exercised through upfront framing and constraints before the main generation step. The artifact chain runs:

> Conversations → Epistemic Traces → Prompt Development Log → Complete Prompt → Output

**Example:** The LinkedIn Post in this repo. Heavy work happened before generation: exploratory conversations produced insights, epistemic traces captured what mattered, a prompt development log tracked how constraints evolved, and the complete prompt specified exactly what to generate.

### Iteration-first

Control is exercised through evaluation and redirection after drafts are produced. The artifact chain includes:

> Specification → Drafts → Evaluation/Redirection → Modification Log → Final Output

**Example:** The companion repo [epistemic-commons-ai-](https://github.com/MicheleLoi/epistemic-commons-ai-). Minimal upfront specification; control happened through iterative evaluation and documented redirection.

### The Article itself (hybrid)

The LinkedIn Article used both patterns:
- **Specification work:** Complete prompt development (`02_complete_prompt/`, `03_prompt_development_log/`)
- **Iteration work:** Post-draft revisions documented in a modification log (`04_modification_log/ModificationLog_LinkedInArticle.md`)

Both patterns document the process as it happens. The difference is where human judgment is concentrated.

---

## Artifact Types

This project shows what engagement evidence can look like. Each artifact type serves a different function:

### Conversations (raw transcripts)
`00_Conversations/`

Preserved AI interactions with metadata. Show the actual exchanges, including contestation, redirection, and the user's organic additions.

### Epistemic Traces
`01_epistemic_traces/`

Structured summaries of what each conversation produced. Capture understanding formed, key sentences that emerged, and how ideas transformed. Enable retrospective analysis without re-reading full transcripts.

### Prompt Development Log (PDL)
`03_prompt_development_log/`

Documents how a prompt evolved through iterations. Critical function: surfaces what got lost in compression and how it was recovered. PDL-002 and PDL-003 in this repo show content from early conversations that was compressed out of intermediate notes, then recovered via epistemic trace review.

### Complete Prompt
`02_complete_prompt/`

Final actionable specification with explicit source mapping. Shows exactly where each element came from in the chain.

### Process Note
`09_notes/Process Note - Artifact Chain Documentation.md`

Documents the full chain with verified text transfers and line numbers. The smoking gun evidence that the development process is reconstructible.

### Modification Log
`04_modification_log/`

Records revisions to outputs after initial generation: what changed, why it changed, and the rationale. Used in the iteration-first pattern to document evaluation and redirection.

---

## Start Here

**If you came from the LinkedIn Post:** Start with the **Prompt Development Log**. PDL-002 and PDL-003 show the lost-and-recovered pattern—content that was compressed out of intermediate notes and recovered via epistemic trace review. Then look at **Epistemic Trace 004** to see where the hinge sentence ("if that capacity is real, it leaves traces") emerged. The **Process Note** ties it all together with line-by-line transfer evidence.

**If you came from the LinkedIn Article:** The Article describes two patterns and points to two repos as examples. This repo shows the specification-first pattern (see the Post's artifact chain). The companion repo [epistemic-commons-ai-](https://github.com/MicheleLoi/epistemic-commons-ai-) shows iteration-first. The Article itself used both — see `02_complete_prompt/` and `03_prompt_development_log/` for specification work, and `04_modification_log/` for post-draft revisions.

---

## The Chains

**Post (specification-first):**
Four conversations → five epistemic traces → prompt development log → complete prompt → published post.

**Article (hybrid):**
Specification work (conversations, epistemic traces, prompt development) → initial draft → evaluation/redirection → modification log → published article.

For the Post's full diagram with transfer evidence, see the **Process Note**.

---

## Why This Exists

The LinkedIn Article makes a claim: meaningful human control can be maintained through either specification-first or iteration-first workflows, as long as the process is documented as it happens.

This repository demonstrates specification-first (the Post) and a hybrid approach (the Article). The companion repo demonstrates iteration-first. All leave traces.

---

## Related

Based on artifact ontology from [The Journal of Prompt-Engineered Philosophy](https://arxiv.org/abs/2504.08579) (arXiv:2504.08579).
