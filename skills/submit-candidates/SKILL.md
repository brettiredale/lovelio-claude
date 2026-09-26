---
name: submit-candidates
description: Send candidates on a Lovelio job to the client, chase the client, and record what the client said. Use when a recruiter wants to submit, float or send candidates to a client, or tells you the client's feedback.
---

# Submit candidates to the client

1. Confirm the job and the candidates with the recruiter. List them with `list_applications` for the job.
2. Send them with `create_submission`, passing the applications as `items` with a short summary for each, written in the recruiter's words. The client gets a link to request interviews, pass or ask questions. The candidates move to Submitted.
3. Check where a submission stands with `list_submissions` or `get_submission`. If the client has gone quiet, `chase_submission` sends a reminder.
4. When the client gives feedback by phone or email instead of their link, record it with `record_client_verdict`: interview requested, or rejected with their reason.
5. To book a client interview, use `schedule_interview`. The candidate moves to Client Interview.

Never name the client in anything written for candidates unless the recruiter asks.
