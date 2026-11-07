---
name: orch-phase-plan
description: Use at the start of each phase (Discovery, Validation, Build) to break the goal into small tasks with owners, budget and a run limit.
---
# Input
The Board's decision from the previous gate (goal, budget, deadline) and the artifacts from the previous phase.

# Artifacts required at each gate
| Gate | Artifacts | Owner → reviewer |
| --- | --- | --- |
| G1 Worth testing? | Opportunity Brief with scorecard | Analyst → Red Team |
| | Red Team memo | Red Team → Board |
| | G1 checklist | CEO (`studio-gate-checklists`) → Board |
| G2 Does anyone want it? | Demand test plan with thresholds (set before the test!) | Analyst → Red Team, approved by Board |
| | Landing test page | Engineer → Board (publishing needs Board approval) |
| | Test results + interview summary | Analyst → Red Team |
| G3 Launch? | MVP spec | Analyst → Engineer (feasibility), approved by Board |
| | MVP on staging + tests | Engineer → Board (acceptance against criteria) |
| | Launch checklist (security, legal, costs) | Engineer + CEO → Board |

# Steps
1. 1–3 tasks per artifact. Each has: owner, reviewer (a different role), definition of done, idea project, deadline, limit of 3 runs, budget limit.
2. Order and dependencies; at most 3 agents working in parallel.
3. Split the phase budget across tasks, keep a 15% reserve.

# Output
Tasks in Paperclip + a phase plan in the parent task (goal, artifacts, order, budget, gate deadline).

# Rules
A task that needs more than 2 runs — split it. Do not create tasks for roles that do not exist.
