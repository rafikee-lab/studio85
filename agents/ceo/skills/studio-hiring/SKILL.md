---
name: studio-hiring
description: Use when work needs a role the studio does not have yet — check the hiring plan and prepare a hiring request for the Board.
---
# Hiring plan
| When | Role | Model |
| --- | --- | --- |
| Start | CEO, Analyst, Red Team | CEO cheaper; Red Team a different model than Analyst |
| After G1 = go | Engineer | strong |
| When the 1st product has paying customers or personal data | QA, DevOps, Security Tester | per studio document |
| When there is something to promote | Growth, Content & Social | per studio document |
| When 2+ products are live | CFO, Compliance, Support, Studio Ops | per studio document |
Until then finance, legal and security = `studio-gate-checklists`; QA = Board acceptance.

# Steps
1. Check whether the moment in the table has come. If not — use a checklist or wait.
2. Request (`studio-escalation`): role, why now, model, monthly budget, manager, minimal permissions.
3. After Board approval, create the agent (`paperclip-create-agent`) with the instructions and skills provided by the Board.

# Rules
No hiring without Board approval. Agents that read a lot of web content get no secrets and no external write actions.
