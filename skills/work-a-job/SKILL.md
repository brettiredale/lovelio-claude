---
name: work-a-job
description: Review and move candidates on a Lovelio job, from the funnel through screening. Use when a recruiter asks what is happening on a job, who is new, or asks to move, shortlist or reject candidates.
---

# Work a job

1. Find the job with `list_jobs`, then read it with `get_job_summary`.
2. List who is on it with `list_applications` filtered by the job. New people sit in Funnel until a person marks them Yes, No or Maybe.
3. Lovelio's own assessment of a candidate is a suggestion. Show it, but never move a candidate because of it. Move someone only when the recruiter tells you to.
4. Move a candidate with `move_stage`. Reject with `reject_candidate`, and pass the reason if the recruiter gives one. For several at once, use `bulk_reject`.
5. To email a candidate, draft it with `prepare_compose_email` and show the draft. Nothing is sent until the recruiter says yes and you call `confirm_email_draft`.
6. Add anything the recruiter tells you about a candidate with `add_note`.

Stages after Screen (Submitted, Client Interview, Offer, Placed) are driven by what happens with the client. See the submit-candidates and log-a-placement skills.
