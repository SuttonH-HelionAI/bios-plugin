---
name: weekly-business-review
description: Give the founder a short review of their store's last 7 days from BIOS, then what is waiting for their yes.
---

Use this when the founder asks how the business is doing, for a weekly review, or for a catch-up.

1. Call `get_business_snapshot` with `range` set to `7d`.
2. Report revenue, orders, average order and ad spend in plain words, and compare with the period before when BIOS gives it.
   - If BIOS says a number is unavailable, say so and say which source did not answer. Never estimate, fill in, or round a missing number to zero.
3. Call `list_approvals`. Name what is waiting, who on the team proposed it, and why, in one line each.
   - Say that deciding happens in the BIOS app (BIOS › Approvals). Do not tell the founder anything was approved, sent or changed.
4. End with at most two suggestions. A suggestion that needs work goes through `request_work` only if the founder says yes to it here.
