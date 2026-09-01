# S1 gate decision — 2026-09-02

Decision authority: user (sole operator, ripple0129@gmail.com) delegated the review to
Claude on 2026-09-01 (「要真人review的部分由你來完成」). Three independent adversarial
reviewers each examined one sample's full before/after files and patch, and
independently re-grepped the runtime vocabulary.

## Decision: **REQUEST CHANGES** (one sample), per gate rules — do not start the bulk rewrite yet

### Sample verdicts

- **curriculum-planner — APPROVED.** Faithful rewrite; pedagogy, confirmation gates,
  and quality checks preserved; zero runtime vocabulary; no fabricated-artifact claims.
- **understanding-by-design — APPROVED.** All UbD/WHERETO concepts intact; clean
  generalization of product object types.
- **k12-core-literacy-planning — CHANGES REQUESTED** (details below).

### Required adjustments for k12-core-literacy-planning

1. **Undisclosed pedagogy loss (primary reason):** upstream ships
   `references/core-literacy.md` + `references/subjects/*` — 229 lines of 2022 课标
   dimension tables, per-subject stage arcs and misconception inventories, containing
   **zero** runtime vocabulary. Nothing in the rewrite rules required removing them.
   Port these reference files into the companion (they are the differentiating content
   vs the sibling understanding-by-design skill).
2. **Self-contradiction introduced:** the rewrite tells the agent to "use general
   core-literacy language" when no standard text is available — but the standard text
   *was* available upstream and was dropped. Restoring (1) resolves this.
3. **Orphaned quality checks:** lines requiring "the central misconception is handled"
   and diagnostics "built from real misconceptions" depend on the dropped misconception
   inventories. Restore (1) or rewrite the checks.
4. **Rule-3 residue:** bare `page`/`deck` nouns survive at lines 45, 60, 63, 82, 87,
   116, 117, 127, 172 — generalize to lesson steps/segments consistently.
5. **Completion-discipline drop:** upstream's "do not stop after presenting a plan"
   turn-ending contract was removed; port a chat-appropriate equivalent (a turn ends
   after explicit learner confirmation or when the stage passes the checks).
6. **Missing-capability path:** the refusal to claim slides/media exist is correct but
   offers no positive fallback — add "offer the content inline in chat" guidance.

Resubmit this one sample after adjustment; the other two samples are approved and the
rewrite rules themselves are validated. Once the revised k12 sample passes, the bulk
rewrite may proceed under the same rules (with adjustment (1) generalized: bundled
reference files that contain no runtime vocabulary must be ported, not dropped).
