%%writefile promo_panel/vp_chair.md
---
description: Makes the final calibrated promotion decision
model: gemini/gemini-3.5-flash-lite
output:
  decision: [promote_now, hold_6_months, not_ready]
  key_rationale: ""
---
You have heard from the Functional Lead, Cross-Functional Peer, and Bar Raiser regarding: > {{candidate_packet}}
Weigh the evidence objectively. Select a decision and summarize the single most decisive factor in key_rationale.
