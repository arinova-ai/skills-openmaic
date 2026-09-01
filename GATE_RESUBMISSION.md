# S1 K-12 sample resubmission — 2026-09-02

Status: **APPROVED AFTER EXPLICIT RE-REVIEW**. This remains a local companion
checkpoint only. The later approval authorized the selected-set local rewrite,
not catalog import; see `GATE_APPROVAL.md`.

## Immutable inputs

- Upstream: `THU-MAIC/OpenMAIC@dfebbcf33f3a56064129903faeab70a9e4243146`
- Original gate packet: `ba6ed7bc1f50d15a8d63affff9c4c8af9d70524c`
- Request-changes decision SHA-256:
  `1d6f534885440f70f84eb49b0ff0fff767a85f0213478cb36cd5dc1342f36fb4`
- Corrected K-12 content commit:
  `933d507931ee46084608fa3fbcc1f3dab8f0b6b8`
- Corrected `SKILL.md` SHA-256:
  `d666930a1ca1aae5d53a5ec5ce95ba03023e9ffa32474e252cdae7f0f6c7c726`
- Full normalized upstream-to-corrected diff:
  `gate-diffs/k12-core-literacy-planning.patch`

## Response to the six requested changes

1. **Pedagogy/reference loss:** restored all five upstream reference files
   byte for byte: `core-literacy.md` and the humanities, languages,
   mathematics, and science subject guides. Their combined size is 229 lines.
2. **Grounding contradiction:** the workflow now requires the bundled general
   reference and exactly one matching subject guide before planning. A supplied
   current standard remains authoritative where it differs.
3. **Orphaned quality checks:** the restored subject guides again provide the
   misconception inventories used by diagnostic and completion checks.
4. **Runtime-object residue:** the corrected main skill contains zero whole-word
   `page` or `deck` matches. Product-neutral terms such as learning segment,
   activity format, diagnostic check, and teaching materials replace them.
5. **Completion discipline:** the conversation workflow now states the only
   valid turn endings: waiting for explicit teacher confirmation, delivering
   requested inline content for an approved segment, or passing the complete
   lesson checks.
6. **Missing-capability path:** when slides, media, audio, or files cannot be
   created, the agent must offer equivalent content inline and identify what
   the teacher must create or attach.

## Reference integrity

| File | SHA-256 |
| --- | --- |
| `references/core-literacy.md` | `47635d06a4a598b28c22a408f5f218e96dd2eca664ca74c1774bb95c848a47ee` |
| `references/subjects/humanities.md` | `616dfe49b3f8c96c917f81a98d04a23b374f1ec509c6d59ee9874d7656353ccc` |
| `references/subjects/languages.md` | `b88c8350e51ffcaf502ef891e0e69f8351295b550c4fe7202efa595de7327b89` |
| `references/subjects/mathematics.md` | `c6a3867f7eb9546928c7ba08243ac3add5e4ec7a963c745191186565632712b1` |
| `references/subjects/science.md` | `2e2e7589fe7798771e69f95bd8222fe0a87ef8f189e8785a0dc90880353e5047` |

Each companion reference is byte-identical to the corresponding file at the
pinned upstream commit. The targeted runtime-vocabulary expression from
`GATE_REVIEW.md` has zero matches across all three sample trees, including the
restored references.

## Gate outcome

The coordinator explicitly returned `APPROVE S1 SAMPLES` after independently
re-verifying the corrected commit and all six changes. The 14-skill local
selected-set rewrite is complete. Acquisition, promotion, staging, and
production remain separate hard gates.
