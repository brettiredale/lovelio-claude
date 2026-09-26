---
name: find-candidates
description: Find the right candidates in the agency's Lovelio database, for a plain-English brief or for a live job. Use when a recruiter asks who they have for a role, wants a shortlist, or asks "who fits this job".
---

# Find candidates

1. If the recruiter names a job, find it with `list_jobs` and run `match_candidates_to_job` on it. That match uses everything the job requires, so do not rebuild the brief yourself.
2. For a free brief ("Python developers in Leeds, 5+ years"), use `search_candidates` and pass the brief as written.
3. Show the ranked list in the order Lovelio returns it, with the why-them line for each person. Never re-rank the results yourself.
4. To look closer at someone, use `get_candidate`.
5. To put someone on the job, use `create_application` with the `search_query` you used, so the source is credited. Only add people the recruiter picks.

If the database has nobody good, say so plainly. `search_web_candidates` finds people outside the database, but only run it when the recruiter asks.
