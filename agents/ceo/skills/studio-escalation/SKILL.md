---
name: studio-escalation
description: Use whenever a decision belongs to the Board (gates, budgets, hiring, deploys, publishing, spending, user data) — so the request is quick to decide and safe.
---
# When
Every decision on the list reserved for the Board, and every case where you would exceed your permissions.

# Request format (always in this order, content in Polish)
```
What we are approving: <1 sentence>
Biggest risk: <1 sentence>
What happens if refused: <1 sentence>
Recommendation: <yes / no / option>
Cost / budget: <amount or tokens>
Decision deadline: <date and time>
Details: <links to artifacts>
```

# After submitting
- No answer by the deadline → reminder to the Board member's deputy.
- Still no answer → **stop**: the matter waits, nothing happens by default.
- High-impact decisions (killing a product, data breach, spending above the threshold) require both Board members.

# Rules
One decision per request. Do not start work "just in case" before the decision.
