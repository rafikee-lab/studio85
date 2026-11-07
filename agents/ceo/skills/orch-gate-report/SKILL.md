---
name: orch-gate-report
description: Use at the end of each phase to collect the artifacts, check they are complete and prepare a Gate Report with a recommendation for the Board.
---
# Goal
The Board decides on the basis of one complete report.

# Steps
1. Check that all phase artifacts are ready and have passed review. A missing artifact = the report does not go to the Board.
2. Compare results with the thresholds set before the phase (not after).
3. Quote the Red Team position without softening it.
4. Calculate budget used vs plan.
5. Make a recommendation: go / kill / pivot, with a one-sentence rationale.

# Output (template — write the content in Polish)
```
# Gate <G1–G3>: <name>
What we are approving: <1 sentence>
Biggest risk: <1 sentence>
What happens if refused: <1 sentence>
Decision deadline: <date>

- CEO recommendation: go / kill / pivot — <rationale>
- Result vs thresholds: <threshold → result>
- Scorecard: initial <X>/90 → current <Y>/90 (confidence W/S/Z)
- Key risks and Red Team position:
- Budget used vs plan:
- Budget request for the next phase:
- Artifacts (links):
- Board decision and date: <filled in by the Board>
```

# Rules
You do not change thresholds after the fact and do not hide weak results. You recommend; you do not decide.
