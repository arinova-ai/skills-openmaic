---
name: curriculum-planner
title: "系列课规划"
description: Multi-lesson series planning for requests such as 「7 天学 Python」, a four-week onboarding track, a semester unit, or "turn this book into a lesson per chapter". Clarifies the brief, gets explicit sign-off on the full lesson list, then develops the lessons one at a time while preserving progression. Use for a sequence of lessons, not a single lesson however large.
---

# Planning and building a lesson series

A series is a sequence of lessons that a learner takes in order. Three things
matter most: getting the brief straight, getting the user's sign-off on the
whole list, and carrying the series from the first lesson to the last without
losing the thread.

Work entirely in conversation. Ask concise questions, show the complete series
proposal, wait for explicit approval, and then produce structured lesson plans
or lesson content in the format the user requested. Do not imply that a deck,
folder, classroom, file, or other persistent artifact was created unless the
current environment actually provides and successfully uses that capability.

## Clarification is sequential

Two principles shape how you clarify:

- **One round is one message.** Put the two or three related questions for that
  round together, then wait for the user's answer before asking the next round.
- **The rounds themselves are sequential, on purpose.** What you ask second
  depends on what they answered first: you cannot offer 「案例领域偏好：生活化小
  工具 / 办公自动化 / 小游戏」 before you know they have never written code. Two
  or three rounds that each build on the last are how someone who knows the
  subject takes a brief; one giant form is a questionnaire.

## Gate 1 — Clarify, in rounds

A series request is almost always underdetermined. A single sentence like
「7 天学 Python」 fixes the topic and the lesson count and leaves open everything
that decides what the lessons actually contain. Work through it in **two or three
rounds**, each round narrower than the one before.

**Round 1 — where this lands.** The two or three things nothing else can be
decided without:

- **who the learner is** — absolute beginner, someone who codes in another
  language, a team with mixed levels;
- **what they want out of it** — a working script of their own, an exam they have
  to pass, a concept they can hold up in a meeting.

Put the example inside the option label: 「完全零基础，没写过一行代码」 tells the
user what you mean by beginner, 「初级」 makes them guess.

**Round 2 — the shape, fitted to Round 1's answers.** Now ask what Round 1 made
askable: how long one session is, the pace, the language of instruction, how
hands-on it should be. **Build the options out of what they just told you** —
「零基础」 turns into 「案例领域偏好：生活化小工具 / 办公自动化 / 小游戏」, and
「平时写 Java」 turns into 「从 Python 与 Java 的差异切入，还是从语法从头讲一遍」.
An option set that could have been written before their answer is the giveaway
that this is a form and not a conversation.

**Round 3 — the edges, and only when they are real.** Whether a book, syllabus or
deck they already have should be the source the series is built from; how much
checking they want (a quiz per lesson, one at the end, none). Skip this round
whenever neither question would change the plan.

Rules that hold for every round:

- **At most three big things per round.** A round carrying six questions is the
  giant form again, wearing three hats.
- **Open each round by saying what you took from the last one.** «既然是零基础、
  每天 30 分钟，我把每课压到一个当天能跑起来的小工具» — the user has to see their
  answer being used. This is the whole reason several rounds read as professional
  rather than slow: a round that does not visibly consume the previous answers is
  just a second form.
- **Never ask what you already know.** Anything the request settled, or that you
  can safely default, is **stated as your decision for them to overrule** rather
  than asked: 「默认中文讲授、每课 30 分钟，要改直接说」 costs no round at all.
- **Two or three rounds, not four.** Opening a round to ask something you could
  have decided yourself is padding, and padding reads as stalling, not as care.
  When the next round has nothing load-bearing left in it, go to Gate 2.

Ask the questions directly and make them easy to answer. Do not bury them in a
long preamble, and do not continue as though silence were consent.

When the request is already specific enough — the user described the audience
and the shape they want, or attached the syllabus — skip this gate. Go straight
to a proposal and let Gate 2 be the one place they confirm.

## Gate 2 — The confirmation gate

**Never start building before the user has signed off on the full series.** A
series of seven stages is seven times the work of one stage; the user has to
see the whole plan before anything is built. This is its own
round, after the clarification rounds are done — never folded into one of them,
because a plan proposed before the answers are in is a plan built on guesses.

Present, in the chat, before any stage exists:

- the **series title** and the **number of stages**;
- **every stage, one line each**: its title and, in a clause, what it is for and
  what the learner can do at the end of it;
- anything you decided for them that they might disagree with — the level you
  pitched it at, the order, what you deliberately left out.

Ask for an explicit go and offer the obvious alternatives to a plain yes:
change the count, reorder, drop or add a lesson, or adjust the level. A silent
or ambiguous answer is not a go. If the user changes something, show the revised
list and ask again. A second confirmation round is far cheaper than seven
lessons built to the wrong brief.

## Designing the series

- **Progression.** Each stage opens where the previous one closed. What is
  assumed to be known must have been taught, in an earlier stage, in a form the
  learner will recognize.
- **Self-contained lessons.** Every stage must stand on its own as a class: a
  learner who takes only day 4 gets a complete lesson with its own opening, its
  own payoff, and enough framing to make sense. A lesson that only works as the
  continuation of another is not a lesson, it is half of one.
- **Review hooks.** From the second stage on, open by reactivating what the
  learner needs from earlier — briefly, and as use rather than repetition:
  apply the earlier idea to the new problem instead of restating it.
- **Difficulty curve.** Difficulty rises steadily and never jumps. Watch for the
  usual failure: three easy lessons, then one that carries the whole hard part.
  If one lesson is doing too much, split it and say so at Gate 2 — the lesson
  count is a proposal, not a constraint the user imposed.
- **Titles that say what the lesson does**, in the series' own language, so the
  folder reads as a curriculum: 「第 3 天：把重复的活写成函数」 rather than
  「Python 基础（三）」.

## The development loop

Once you have the go:

1. Restate the approved series title, audience, outcome, cadence, and lesson
   list as a compact working contract.
2. Develop each lesson in order. For every lesson provide its outcome,
   prerequisites, opening hook, teaching sequence, learner practice, evidence
   of learning, transfer task, and bridge to the next lesson.
3. After each lesson, write one short paragraph explaining what it actually
   covered and what the next lesson may safely assume. Use the completed lesson,
   not only the original proposal, as the continuity record.
4. If the user requested full learner-facing content, produce it lesson by
   lesson and label unfinished portions plainly. If they requested a curriculum
   plan, do not inflate it into invented completed materials.

## Long-run context discipline

A series is a long conversation. Your per-lesson recap is the series' memory:
keep it about what the lesson teaches, what it assumes, and what it leaves for
later. Do not re-quote outlines already summarized or restate the whole series
plan at every step. Consult the earlier messages when continuity depends on a
detail rather than reconstructing it from memory.

## When something fails

One weak or incomplete lesson does not end a series. If part of a lesson cannot
be completed from the available information:

- ask for the missing fact when it is load-bearing; otherwise mark a bounded
  assumption and continue;
- leave the rest of that lesson intact and move on when useful independent work
  remains. Do not restart the series or silently drop a lesson from the plan;
- keep a short running list of what did not come out right, and **report it at
  the end**: which lesson, which section, and what still needs revision.

## Finishing

Close with:

- a short **series summary**: the lessons that were built, in order;
- links only to artifacts that really exist;
- the **rework list** — anything incomplete or worth revising — or a sentence
  saying there is none.

## Related skills

If a lesson has a distinct shape—hands-on, vocational, or research-backed—use
the relevant teaching approach inside that lesson. Verify any time-sensitive or
specialist facts **before Gate 2**, not after: a series plan the user approved is
a plan you then have to honor.
