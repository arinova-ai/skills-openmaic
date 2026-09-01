# S1 local selected-set rewrite checkpoint — 2026-09-02

Status: **LOCAL COMPANION REWRITE AND AUDIT PACKET COMPLETE; CATALOG PROMOTION
NOT STARTED**.

## Immutable inputs and decisions

- Upstream:
  `THU-MAIC/OpenMAIC@dfebbcf33f3a56064129903faeab70a9e4243146`
- Original gate packet:
  `ba6ed7bc1f50d15a8d63affff9c4c8af9d70524c`
- Corrected K-12 content:
  `933d507931ee46084608fa3fbcc1f3dab8f0b6b8`
- Bulk content:
  `97db4a2823591e402b59463c1d5866a506eabf36`
- Deep-research boundary:
  `0f5d13daca153219812d39bf3dc83f03dcf03a95`
- Approval and authorization: `GATE_APPROVAL.md`
- Authoritative disposition list: `SELECTION.md`

## Applied local scope

- Selected pedagogy skills: 14.
- Excluded product/authoring/DSL agent-runtime entries: 9.
- Auxiliary files: 11, all present at their corresponding companion paths and
  byte-identical to the pinned upstream files.
- `BULK_MANIFEST.tsv` records every selected skill and auxiliary path plus its
  upstream and companion SHA-256.
- `EVIDENCE_HASHES.tsv` pins this approval/selection/checkpoint packet and all
  11 normalized bulk patches by SHA-256.
- `gate-diffs/` contains the three approved sample patches.
- `bulk-diffs/` contains 11 zero-context, CRLF-normalized semantic patches for
  the remaining selected skills. Each patch applies cleanly to a temporary copy
  of its pinned upstream source and reproduces the companion file.

## Verification contract

The local checkpoint must reproduce all of the following before handoff:

- manifest rows: 14 skills and 11 references; path/hash mismatches: 0;
- selected/excluded disposition counts: `14 / 9`;
- selected frontmatter `name` mismatches: 0;
- targeted runtime-vocabulary matches across `skills/`: 0;
- K-12 bare whole-word `page`/`deck` matches: 0;
- auxiliary byte mismatches against pinned upstream: 0;
- normalized bulk patches: 11, apply/reproduction failures: 0;
- evidence-file SHA-256 mismatches: 0;
- symlinks: 0;
- `gitleaks detect --no-git --source . --redact --exit-code 1`: no leaks;
- `git diff --check` and evidence-commit `git show --check`: clean.

## Hard gates

This checkpoint does not create a catalog candidate or certify a canonical
dry-run. Catalog acquisition/promotion waits for the coordinator's finish-3
exact SHA and explicit phase authorization. Push, PR, staging, and production
are outside this checkpoint.
