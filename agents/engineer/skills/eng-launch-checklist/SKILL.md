---
name: eng-launch-checklist
description: Use before G3 to check the MVP's minimum security and production readiness.
---
# Checklist
- [ ] No secrets in the repo (scan), secrets in the secret manager
- [ ] Dependency scan with no critical vulnerabilities; versions pinned
- [ ] Auth and permissions from a ready-made service; users see only their own data
- [ ] Input validation, protection against common attacks (OWASP Top 10), rate limits on forms
- [ ] HTTPS, security headers
- [ ] Separate environments and keys for staging and production
- [ ] Logs free of personal data and secrets
- [ ] Database backup + one test restore
- [ ] Monitoring: is the site up, alert to the Board
- [ ] Monthly cost of infrastructure and services
- [ ] If the product uses AI with users: labelling and protection against prompt injection in user data
# Output
Table: item | OK / gap | action. Every "gap" = a task or a conscious Board decision.
