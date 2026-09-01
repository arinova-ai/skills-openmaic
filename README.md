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

## Approved local companion scope

This checkpoint contains 14 approved, rewritten pedagogy skills. The three
initial samples were:

1. `curriculum-planner`
2. `k12-core-literacy-planning`
3. `understanding-by-design`

The full set is enumerated in [`SELECTION.md`](SELECTION.md). All 14 preserve
the reusable upstream pedagogy and replace unavailable calls such as
`create_stage`, `generate_scene`, `patch_stage`, `set_roster`, `ask_user`, and
`edit_deck` with ordinary conversation, explicit confirmation, and structured
lesson outputs. Following the 2026-09-02 request-changes decision, the K-12
sample also carries its five upstream core-literacy reference files (229 lines)
and the six-item response is documented in `GATE_RESUBMISSION.md`. The later
approval and full-set review are documented in `GATE_APPROVAL.md`; the complete
path/hash and normalized-diff evidence is in `BULK_MANIFEST.tsv`,
`EVIDENCE_HASHES.tsv`, `BULK_REWRITE.md`, `gate-diffs/`, and `bulk-diffs/`.

Exactly 9 product/authoring/DSL entries (`build-personal-skill`, `page-clone`,
`pptx-import`, `pro-editing`, `slide-craft`, `slide-dsl`, `stage-design`,
`stage-dsl`, and `style-clone`) are outside this companion's selected set. No
catalog acquisition, promotion, staging, or production action has been taken.
