---
name: plan-a-campaign
description: Help the founder shape a marketing campaign with their store's real numbers, then hand it to their BIOS team to propose.
---

Use this when the founder wants a promotion, a sale, an email campaign or an ad push.

1. Ask what they want to achieve and by when, if they have not said.
2. Ground the plan in their numbers: call `ask_bios` (for example "revenue last 30 days") or `get_business_snapshot` with `range` `30d`. Use only numbers BIOS returns; if one is unavailable, plan without it and say so.
3. Agree a short brief with the founder: the goal, the offer, who it is for, the channel, and the dates.
4. Only after the founder says to go ahead, call `request_work` with the brief in plain words.
5. Tell the founder their BIOS team will plan the campaign in BIOS, and that any send or spend it proposes waits for their yes in the BIOS app.
