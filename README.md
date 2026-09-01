# OpenMAIC pedagogy skills companion

This repository adapts the pedagogy-focused skills from
[`THU-MAIC/OpenMAIC`](https://github.com/THU-MAIC/OpenMAIC) into self-contained
conversation workflows that do not depend on the OpenMAIC stage/deck runtime.
The source material is primarily Simplified Chinese with English frontmatter.

## Provenance and license

- Upstream repository: `https://github.com/THU-MAIC/OpenMAIC`
- Reviewed upstream commit: `dfebbcf33f3a56064129903faeab70a9e4243146`
- Upstream project and author attribution: THU-MAIC / OpenMAIC contributors
- License: MIT; the complete upstream license is retained in [`LICENSE`](LICENSE)

## Human review gate

This checkpoint contains exactly three rewritten samples:

1. `curriculum-planner`
2. `k12-core-literacy-planning`
3. `understanding-by-design`

They preserve the upstream pedagogy and replace unavailable calls such as
`create_stage`, `generate_scene`, `patch_stage`, `set_roster`, `ask_user`, and
`edit_deck` with ordinary conversation, explicit confirmation, and structured
lesson outputs. Following the 2026-09-02 request-changes decision, the K-12
sample also carries its five upstream core-literacy reference files (229 lines)
and the six-item response is documented in `GATE_RESUBMISSION.md`. Full-batch
adaptation and catalog import must not begin until the corrected sample is
explicitly approved.

Authoring/DSL entries (`slide-dsl`, `stage-dsl`, `page-clone`, `pptx-import`,
and related runtime tooling) are outside this companion's scope.
