# S1 human gate: three OpenMAIC rewrites

Status: **RESUBMITTED AFTER REQUEST CHANGES; WAITING FOR EXPLICIT USER
APPROVAL**. The original decision is preserved in [`GATE_DECISION.md`](GATE_DECISION.md),
and the six-item response is recorded in
[`GATE_RESUBMISSION.md`](GATE_RESUBMISSION.md). This packet still contains only
the three required samples. No bulk rewrite has been started.

## Provenance and review snapshot

- Upstream: `https://github.com/THU-MAIC/OpenMAIC`
- Upstream commit: `dfebbcf33f3a56064129903faeab70a9e4243146`
- License: MIT (`LICENSE` is preserved at the companion repository root)
- Companion: `https://github.com/arinova-ai/skills-openmaic`
- Original sample-content commit: `f05dbdf309199dd2072a9026660171a0003ea9a0`
- K-12 corrected-content commit: `933d507931ee46084608fa3fbcc1f3dab8f0b6b8`
- Local upstream root: `/Users/ripple/skill-gap-2-upstreams/S1-openmaic`
- Local companion root: `/Users/ripple/orca/workspaces/arinova-skill-companions/skills-openmaic`

The patch files in `gate-diffs/` compare the exact upstream file at the pinned
commit with its proposed companion file at the sample-content commit. Line
endings are normalized in the patches only so that reviewers see semantic
changes instead of CRLF noise.

## Rewrite rules applied to all three samples

1. Preserve the learning theory, learner outcomes, instructional sequence,
   explicit confirmation gates, quality checks, source language, and English
   frontmatter fields.
2. Replace OpenMAIC-only stage, deck, page, roster, and tool orchestration with
   ordinary chat questions, an explicit wait for confirmation, and structured
   chat output. Never claim that a persistent artifact was created.
3. Generalize product-specific slide, interactive, quiz, and PBL object types
   into lesson steps, activities, diagnostics, and performance tasks.
4. Preserve bounded failure and degraded-mode guidance. Do not introduce a new
   vendor or runtime dependency.
5. Exclude authoring/import/DSL skills from the later bulk set rather than
   trying to disguise product-specific mechanics as generic pedagogy.
6. Port bundled reference files that contain no targeted runtime vocabulary;
   do not discard pedagogical grounding merely because the runtime wrapper is
   removed.

The targeted runtime vocabulary check was:
`create_stage|generate_scene|patch_stage|set_roster|ask_user|edit_deck|stage-design|pro-editing|OpenMAIC|` followed by the product object names
`slide`, `interactive`, `quiz`, and `pbl` in backticks. Each proposed sample has
zero remaining matches.

## Sample 1: curriculum-planner

- Before: `/Users/ripple/skill-gap-2-upstreams/S1-openmaic/skills/agent-runtime/curriculum-planner/SKILL.md`
- After: `/Users/ripple/orca/workspaces/arinova-skill-companions/skills-openmaic/skills/curriculum-planner/SKILL.md`
- Full diff: `gate-diffs/curriculum-planner.patch`
- Before SHA-256: `9a3b68cf38523d7930fecc24266e8ed9d2f7342447a525ec64d26c66594c6ac5`
- After SHA-256: `3fd9b27eb7676ca29626e592fd34053231c31e54b10715b1881b8300ba70b4f4`
- Size/diff: 212 lines before, 178 after; `+54/-88`
- Targeted runtime terms: 18 before, 0 after

Difference summary: removes the product-specific “`ask_user` ends the run”
contract and stage-generation loop, while keeping sequential clarification,
the full-series confirmation gate, cross-lesson progression, and quality
review. The proposed version uses a normal chat workflow and explicitly avoids
claiming that a folder, deck, classroom, or file was created.

## Sample 2: k12-core-literacy-planning

- Before: `/Users/ripple/skill-gap-2-upstreams/S1-openmaic/skills/agent-runtime/k12-core-literacy-planning/SKILL.md`
- After: `/Users/ripple/orca/workspaces/arinova-skill-companions/skills-openmaic/skills/k12-core-literacy-planning/SKILL.md`
- Full diff: `gate-diffs/k12-core-literacy-planning.patch`
- Before SHA-256: `fbc03e9245406bac2d5b312f1a5711de311d17dc98eeb30d8eab298ee397c08f`
- After SHA-256: `d666930a1ca1aae5d53a5ec5ce95ba03023e9ffa32474e252cdae7f0f6c7c726`
- Size/diff: 185 lines before, 195 after; `+79/-63`
- Targeted runtime terms: 26 before, 0 after

Difference summary: replaces `create_stage`, `ask_user`, `generate_scene`,
`patch_stage`, and `edit_deck` calls with a conversational lesson-plan
workflow. It preserves literacy load planning, assessment, accessibility,
learner context, and both new-plan and existing-plan paths. The corrected
sample also ports the five upstream core-literacy reference files byte for
byte (229 lines), consults them before planning, removes the remaining generic
runtime-object residue from the main skill, restores the turn-ending contract,
and offers inline chat content when slide or media capabilities are absent.

## Sample 3: understanding-by-design

- Before: `/Users/ripple/skill-gap-2-upstreams/S1-openmaic/skills/agent-runtime/understanding-by-design/SKILL.md`
- After: `/Users/ripple/orca/workspaces/arinova-skill-companions/skills-openmaic/skills/understanding-by-design/SKILL.md`
- Full diff: `gate-diffs/understanding-by-design.patch`
- Before SHA-256: `75af8be3ec7772b6ae97ac70ceedbb00fcfbb16a6d4addceb5f62ec0b3614808`
- After SHA-256: `52b4e42f2768347d5ea10460452ee230ee1157bc2a0cf2e84c94397576598a13`
- Size/diff: 70 lines before, 70 after; `+18/-18`
- Targeted runtime terms: 21 before, 0 after

Difference summary: replaces OpenMAIC object types and stage-editing calls
with ordinary clarification, GRASPS performance tasks, diagnostics, learning
activities, and existing-plan adaptation. All UbD and WHERETO concepts remain.

## Decision requested

Please re-review the corrected K-12 sample and explicitly choose one of these
outcomes:

- **APPROVE S1 SAMPLES** — apply these rules to the full selected S1 set.
- **REQUEST CHANGES** — identify the sample and requested adjustment; do not
  start the bulk rewrite.

Silence, a passing scan, or approval of another package does not pass this
gate.
