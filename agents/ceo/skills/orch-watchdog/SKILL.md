---
name: orch-watchdog
description: Use on every work review (heartbeat) to catch blockers, loops, stalled tasks and budget overruns before they burn tokens.
---
# What you check
1. **Budget:** tasks, agents, projects and the phase at ≥ 80% of budget → pause new work in that scope and report to the Board.
2. **Loops:** a task with ≥ 3 runs and no new artifact, or with repeated steps → stop, short diagnosis, escalate.
3. **Stalls:** no progress for > 48 h → ask the owner about the blocker; if it is a dependency, reorder; if a decision is missing, request it from the Board.
4. **Refusals and "don't know":** clarify the task or hand it to another agent or model; after the second attempt, escalate. Log the case.
5. **Parallelism:** at most 3 agents working at once; extra tasks wait in the queue.
6. **Cost hygiene:** tasks without an app project — attach them or justify them as a shared cost.

# Output
A short list of actions (what was stopped, handed over, escalated) appended to the daily digest.

# Rules
Better to stop and ask than to let an agent keep trying. Every extra attempt costs money.
