![Lovelio](icon.svg)

# Lovelio for Claude

Lovelio is the ATS for recruitment agencies. This plugin connects Claude to your agency's Lovelio account, so you can run your desk in plain English: find candidates for a job, work the shortlist, send candidates to a client, chase the client, and log offers and placements.

## What is in it

- **Connector**: the Lovelio MCP server for your region, signed in with OAuth. Claude acts as you, with your Lovelio permissions, and every change shows in the activity log like any change you make in the app.
- **Skills**: four recruiter workflows. `find-candidates`, `work-a-job`, `submit-candidates` and `log-a-placement`.

## Set up

1. Install the plugin.
2. Connect the server for the region you sign in on. Your workspace lives in one region, and a sign-in only works there.

| Server | Sign-in domain |
|---|---|
| `lovelio-us` | us.lovelio.ai |
| `lovelio-eu` | eu.lovelio.ai |
| `lovelio-anz` | anz.lovelio.ai |

3. Sign in to Lovelio and approve access on the consent page.
4. Ask something like "Who do we have for the Leeds finance manager job?"

## What data it sends

Claude sends your requests and the details you give it (names, job details, notes, emails) to Lovelio's server in your region, and reads back the records your Lovelio permissions allow. Nothing goes anywhere else. Emails and client submissions are only sent when you confirm them. You can disconnect at any time from Settings in Lovelio.

- Docs: https://lovelio.ai/docs/mcp
- Privacy: https://lovelio.ai/privacy
- Terms: https://lovelio.ai/terms
- Support: support@lovelio.ai
