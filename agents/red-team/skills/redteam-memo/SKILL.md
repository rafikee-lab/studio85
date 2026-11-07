---
name: redteam-memo
description: Use before each gate (G1–G3) or to review an Analyst artifact — to point out the idea's weakest points and measurable kill conditions.
---
# Steps
1. Read the artifact and the idea intake form (not the whole thread).
2. Forcing questions — check whether the artifact answers them specifically:
   - **Real demand:** what is the strongest evidence someone really wants this (pays, changes how they work), not just "is interested" or joined a waitlist?
   - **Status quo:** what do people do today, even badly, and what does it cost them? "They do nothing" = the problem is probably not painful enough.
   - **Specific person:** who exactly (role, situation, consequence), not a category ("SMBs", "parents")?
   - **Narrowest wedge:** what is the smallest version someone would pay for this week?
3. Pre-mortem: "It is a year later and the idea failed. Why?" Sort the risks into:
   - **Tigers** — real, backed by evidence or clear logic
   - **Paper tigers** — look scary but are overblown (say why)
   - **Elephants in the room** — nobody talks about them, yet they may be real
   Before G3, split tigers into: launch-blocking / within 30 days of launch / monitor.
4. Check: who really pays; can a big player copy it easily; is the acquisition channel real and cheap; legal risks and dependency on one platform; are the test thresholds too lenient.
5. Randomly verify 3 sources.

# Template (write the content in Polish)
```
# Red Team: <name> — <gate>
## Forcing questions: question | answer in the artifact | rating: specific / vague / missing
## Tigers (most serious first): risk | evidence | how to settle | (G3: blocking / 30 days / monitor)
## Paper tigers: risk | why overblown
## Elephants in the room: what | how to investigate
## The assumption most likely to be false
## Source check: 3 links | OK / problem
## I recommend kill if: <measurable conditions>
## Overall: weak / to verify / strong — 1 sentence
```
# Red flags
"People say it's interesting", "500 waitlist sign-ups", "the market is huge", "nobody does this" — none of these is evidence of demand.
Inspired by: YC office hours (garrytan/gstack, MIT), pre-mortem (phuryn/pm-skills, MIT).
