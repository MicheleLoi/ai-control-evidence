# Modification Log: LinkedIn Article (2026-01-21)

**Document:** `LinkedIn-Article-2026-01-21.md`
**Date:** 2026-01-19
**Purpose:** Document revisions to the LinkedIn Article on meaningful human control.

---

## Revision 1: Terminology clarification

**Issue identified:** The original framing used "before-generation" vs "after-generation" terminology, which created two ambiguities:

1. **Timing ambiguity:** It sounded like the distinction was between documenting *before* vs *after* AI involvement—i.e., ex ante vs ex post documentation. That is not the distinction. Both patterns document the process as it unfolds (both are ex ante).

2. **Draft/output conflation:** By implying the first AI draft is "the generation," the framing confused intermediate drafts with the final product.

**Actual distinction:** The two patterns differ in *where human control is exercised*:
- **Specification-first:** Control through upfront framing and constraints before drafting
- **Iteration-first:** Control through evaluation and redirection after drafts are produced

Both produce documentation as the work happens. The locus of judgment differs, not the timing of documentation.

**Changes made:**

| Location | Original | Revised |
|----------|----------|---------|
| Line 20 (intro sentence) | "two documentation patterns—one 'before-generation,' one 'after-generation'" | "two workflows for maintaining meaningful human control: one where control is exercised through upfront specification, one through iterative evaluation. Both document the process as it happens." |
| Line 22 | "Repo 1 (pre-prompt pattern)" | "Repo 1 (specification-first)" |
| Line 23 | "Repo 2 (post-prompt pattern)" | "Repo 2 (iteration-first)" |
| Line 69 (section header) | "Pattern 1: Pre-prompt documentation (control before generation)" | "Pattern 1: Control through specification" |
| Line 116 | "in a pre-prompt workflow" | "in a specification-first workflow" |
| Line 120 (section header) | "Pattern 2: Post-prompt documentation (control after generation)" | "Pattern 2: Control through iteration" |
| Lines 125-126 | "Instead of doing most structuring before generation, you do it after: the model drafts, the human judges, and iteration is documented." | "Instead of front-loading structure into a detailed specification, this workflow distributes control across drafting cycles: the model produces a draft, the human evaluates and redirects, and the iteration is documented." |
| Line 224 (subheading) | "Pre-prompt pattern is strong when:" | "Specification-first is strong when:" |
| Line 229 (subheading) | "Post-prompt pattern is strong when:" | "Iteration-first is strong when:" |
| Lines 236-237 | "pre-prompt artifacts for framing and scope / post-prompt logs for evaluation and refinement" | "specification artifacts for framing and scope / iteration logs for evaluation and refinement" |

**Rationale:** The new terminology makes explicit that:
1. Both patterns are forms of ex ante documentation (recorded as work happens)
2. The difference is the *locus* of human judgment—specification vs iteration
3. "Draft" and "final output" are not conflated
