---
name: fact-check
title: "事实核查"
description: "Improve factual reliability while creating or reviewing a lesson or supplied content. Use when the user asks to fact-check, verify accuracy, reduce hallucinations, or mentions 事实性错误、知识性错误、专业知识准确性、可靠性. During creation, check completed content before delivery; when reviewing existing material, return a short evidence-backed report and let the user choose what to fix. Not for grammar, style, or layout. Combine with deep-research when current evidence is the lesson's main subject."
---

# Fact check

Keep serious factual mistakes and hallucinations out of learning content
without turning the work into an exhaustive audit. Focus on the few claims that
materially affect trust.

Infer the mode from the request:

- **Creating:** fact-check the completed lesson before delivery and correct
  errors introduced during drafting, subject to the source-of-truth boundary.
- **Reviewing:** report findings first. Do not edit unless fixes were already
  requested or the user approves them after seeing the report.

## Read the entire requested scope

Read the supplied content in order, including visible text, notes, narration,
captions, and answer explanations when available. Respect a narrower scope if
the user gives one. If part of the source cannot be accessed, name the missing
portion rather than claiming a full review.

Read once for context and silently shortlist high-signal risks:

- exact numbers, dates, counts, names, and quotations;
- laws, standards, formulas, technical definitions, and classifications;
- “first,” “only,” “always,” “must,” and other absolute claims;
- causal, medical, legal, financial, or professional conclusions presented as
  settled fact;
- contradictions between sections;
- suspiciously precise claims with no visible support.

Do not verify every sentence. Skip correct material, wording preferences,
harmless simplifications, and low-value trivia.

## Verify only the shortlist

Check relevant user materials first. The content being reviewed cannot prove
itself. Use current web research for shortlisted claims that are exact,
changing, disputed, high-stakes, or specialist. A normal first pass should need
no more than about six to eight searches.

Prefer primary or official sources and read the actual source; a snippet is not
evidence. For versioned knowledge, verify the date, version, and jurisdiction.
For compound statements, isolate and test the questionable part.

If search or source access is unavailable, make fewer factual commitments and
mark important uncertainty. Never guess a URL or fabricate supporting text.
“No reliable evidence found” does not establish falsity.

## Preserve approved inputs

Do not silently correct a claim that materially conflicts with a settled plan,
user-supplied source, or fact the user explicitly approved. Flag the exact
conflict, show concise contrary evidence, and ask the user to choose among:

- keep the approved input;
- authorize the factual correction; or
- review the conflict without editing.

This boundary does not protect an error independently introduced by the
assistant. During creation, correct those errors before delivery.

## Report only useful findings

In review mode, return roughly three to eight material findings on the first
pass, or fewer when fewer exist. Use these groups in order and omit empty ones:

- **A. 明确事实错误**
- **B. 表述不严谨**
- **C. 需要核实**

Number findings across all groups. Give each a short bold line with its number,
location, and issue, such as `**1. 第 5 节｜解析｜知识混淆**`. Under it use
exactly three bullets:

- **原始表述：** quote only the necessary fragment;
- **存在问题：** explain the problem and correct fact, with concise source and
  date when useful;
- **修改建议：** state the edit or a compact replacement.

Keep each bullet to one or two sentences. Do not show scores, confidence
percentages, lengthy method, correct claims, or minor style issues. If no
material problem is found, state the scope reviewed and that no obvious error
was found; never claim perfect accuracy.

## Approval and editing discipline

When review mode finds actionable issues and edits were not pre-authorized,
end by asking the user to choose: fix all reported issues, fix confirmed errors
only, keep the report unchanged, or name specific finding numbers. Wait for the
answer. Then change only the approved claims and read the affected context again
to ensure the correction did not introduce a contradiction.

When creating, mention only material corrections or remaining uncertainty in
the handoff. Do not interrupt the lesson-building flow with a separate approval
gate unless an approved-input conflict requires it.
