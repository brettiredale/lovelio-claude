---
name: log-a-placement
description: Record an offer and a placement in Lovelio, with the fee. Use when a recruiter says a client made an offer, a candidate accepted, or asks to log a placement or a win.
---

# Log an offer and a placement

1. When the client makes an offer, call `log_offer` on the application. It moves the candidate to Offer. The client owns the offer letter; Lovelio just records the stage.
2. When the candidate accepts, call `create_placement` with the `application_id`. The fee percent and guarantee come from the client's standard terms unless the recruiter gives different ones. Ask for the start date and salary or rate if you do not have them.
3. Read it back with `get_placement` and confirm the fee with the recruiter.
4. If the placement falls through later, use `mark_placement_status`.

Check the numbers with the recruiter before you create a placement. It is the agency's billing figure.
