# Weekly Operating Rhythm

Use this document to run the contributor pipeline without turning it into six disconnected spreadsheets. The [PR Tracking Dashboard](https://github.com/code-orange-dev/PR-tracking-dashboard) is the public source for current linked PR outcomes; this record is the private weekly operating layer that explains what happens before a PR exists.

## 60-Minute Developers Call

| Time | Topic | Required outcome |
| --- | --- | --- |
| 0–5 min | Outcome and definitions | Confirm this week's reporting cutoff and the one bottleneck to solve. |
| 5–15 min | Canonical scorecard | Read the funnel, PR states, and stale records; do not debate unlinked metrics. |
| 15–25 min | Active contributor board | Every open PR has a next action, blocker, and mentor or peer-review path. |
| 25–35 min | Graduate / First PR Challenge board | Every participant has one scoped upstream action before the next call. |
| 35–45 min | Fellowship capacity | Confirm mentor seats, project fit, and Month-3/alumni issues before accepting applicants. |
| 45–55 min | Decisions | Lock the metric cutoff, owner assignments, experiment change, and any escalation. |
| 55–60 min | Commitments | Record one owner, one dated next action, and one proof link for every decision. |

### Decisions to make each week

1. Which funnel stage is leaking most: first-session attendance, second-session return, contribution evidence, or PR submission?
2. Which current contributor needs a maintainer, mentor, or peer-review escalation?
3. Which graduate receives the next scoped issue and named mentor?
4. Is mentor capacity sufficient for any fellowship decision this week?
5. What single change will the growth lead test before the next call?

## One Canonical Weekly Scorecard

Use a single dated record with source links. Do not combine pre-Code-Orange contribution history with program-attributed outcomes, and never change a prior week's number without recording why.

| Metric | Definition | Source / verifier | Weekly owner |
| --- | --- | --- | --- |
| Qualified developer joins | New developers who supplied a handle/contact and selected a technical entry path | Registration or Discord record | Growth Lead |
| Intro posts | Qualified joins who posted an introduction | Discord permalink | Growth Lead |
| First technical session | Intro posters attending one technical session | Attendance record | Session Lead |
| Second-session return | First-session attendees who attend another technical session within 30 days | Attendance record | Session Lead |
| Scoped upstream action | Graduates given one verified issue, review, test task, or design task | Graduate roster link | Pipeline Operator |
| Contribution evidence | Linked upstream issue, review, PR, reproducible test artifact, or public demo | GitHub / artifact link | Pipeline Operator |
| PRs open / under review | In-scope submitted PRs that are neither merged nor closed at cutoff | PR dashboard link | PR Verifier |
| PRs merged | In-scope upstream PRs merged at cutoff | PR dashboard link | PR Verifier |
| Active contributors | Dashboard definition, rechecked at the monthly public update | PR dashboard link | PR Verifier |
| Mentor capacity | Confirmed seats, filled seats, and fellows lacking fallback support | Fellowship capacity table | Mentor Lead |
| Fellow milestone status | Green / yellow / red against weekly evidence and Month-3 review | Fellowship record | Fellowship Lead |

Record: `week ending`, `reporting cutoff`, `source links`, `owner`, `next action`, and `next action due` on every row that needs follow-up.

## 90-Day First PR Challenge: Operator Run

The challenge in the main playbook is the marketing promise. This is the weekly execution loop.

### Before launch

- Publish one clear CTA: **"Open your first upstream Bitcoin OSS PR in 90 days."** Link to the current PR dashboard and the next entry session.
- Recruit through one developer community, CS department, or language meetup at a time; include one 60–90 second contributor story with a verifiable PR link.
- Build a small verified issue menu. Each item must name the upstream repo, skill, mentor/office-hour path, and a first action.
- Set a baseline from the immediately previous eight-week intake: first-to-second-session return and 30-day contribution evidence.

### First 48 hours

- Send every attendee one personal follow-up: two lines on what happened, one specific upstream action, and the date of the next session.
- Record their entry path and give them a buddy or office-hour route. No generic “keep learning” messages.
- Ask for an intro post and schedule the second technical session before the first one ends.

### Weekly run (Weeks 1–8)

1. Check the scorecard and contact anyone missing their second session or next action.
2. Run a contribution clinic or office hour tied to the verified issue menu.
3. Publish one proof-of-work update: a participant's issue, review, test, or PR—with their consent.
4. Update the public PR dashboard only through the PR Verifier; do not put unverified claims on the leaderboard.
5. Pay referral or milestone rewards only after the required evidence (for referrals, after the invited developer's second session).

### Decision metrics

Primary metric: **first-session → second-session return**. Secondary metrics: 30-day contribution evidence and 90-day first upstream PR opened. A merge is a lagging metric controlled partly by upstream reviewers.

For the pilot, aim for 60%+ second-session return, 40%+ contribution evidence by day 30, and 25%+ first upstream PRs opened by day 90. Compare with the immediately prior intake; if second-session return does not improve within two months, change format or follow-up rather than increasing promotional volume.
