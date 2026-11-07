---
name: eng-mvp
description: Use after G2 = go to build the MVP according to the approved spec — story by story, with tests, on staging.
---
# Steps
1. Read the spec; report unclear points and feasibility risks to the CEO before you start.
2. Plan: list of stories in order, an estimate for each, external services needed (with cost).
3. For each story: first a test for the acceptance criterion (Given/When/Then), see it fail, then code until it passes.
4. After each story: run the full test suite, deploy to staging, short comment on the task (what works, how to check, test results).
5. At the end: report — criteria met X/Y, known gaps, monthly running cost, acceptance instructions for the Board.

# Evidence before claims
Do not write "works", "done" or "fixed" until you have run the command that proves it in the same run and read the output. Put the evidence in the comment (e.g. "tests: 24/24, 0 failures"). "Should", "probably", "likely" = not yet verified.

# Bugs
Root cause first, then the fix: reproduce, find the source, fix, add a test that catches it. After 3 failed fixes — stop and comment to the CEO.

# Rules
Nothing outside the spec. Every new dependency justified. Test data only, never real data.
Inspired by: verification-before-completion, systematic-debugging, test-driven-development (obra/superpowers, MIT).
