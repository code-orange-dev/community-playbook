# 🟠 The Code Orange Community Playbook

> **How we turn developers into Bitcoin open-source contributors - and how your community can too.**
>
> Written by [Code Orange Dev School](https://codeorange.dev) in Canggu, Bali, from what we do in our own community. Contributions by our community members are tracked, with links, on our [PR dashboard](https://github.com/code-orange-dev/PR-tracking-dashboard).
>
> **License: CC0.** Fork it, translate it, run it in your city. If it helps, tell us - we love seeing this spread.

---

## The philosophy

Three rules make everything else work:

1. **Contribution-first.** Every session ends with a concrete next step in a real repo. Never teach theory without a "do this before next week."
2. **Nobody leaves empty-handed.** Every first-timer walks out with something running - a node, a signet wallet, a merged typo fix. The first session decides whether there's a second.
3. **Sell the career, not the curriculum.** The honest pitch to a developer: *your GitHub becomes your CV, your CV becomes your income.* Open-source contributions lead to fellowships and grants that pay globally - that's a life-changing offer in most of the world, and it's true.

---

## Part 1 - Onboarding that doesn't leak

### Auto-welcome DM (Discord - MEE6, Carl-bot, or a mod)

> Hey {name}, welcome to Code Orange 🟠
>
> Three steps to get started:
> 1. Say hi in #introductions - who you are, what you code (or want to code)
> 2. Pick your entry point:
>    • New to Bitcoin → **Bitcoin Basics** (next: {date})
>    • Can code, new to Bitcoin dev → **Bitcoin Dojo** (next cohort: {date})
>    • Ready for advanced → **Privacy Track** (bi-weekly, drop in any session)
> 3. Full calendar: {link}
>
> Everything is free. The goal: your first node → your first merged PR.

### #start-here pinned message

> **🟠 START HERE**
> Code Orange takes developers from first Bitcoin node → first merged PR → first grant. Free, open-source, contribution-first.
> **This week:** {sessions}
> **The path:** Basics → Dojo → rawBit → Decoding Bitcoin → Privacy Track → Fellowship
> **Proof:** {your PR dashboard link}
> Questions → #general. See you at a session 👇 {calendar}

### The 48-hour rule

Within two days of every workshop, send attendees one message: what was covered (2 lines), one specific action for the week (a good-first-issue link, not "keep learning"), and the next session date. It helps people come back. Template:

> Thanks for joining {workshop}! 🟠
> **What we covered:** {2 lines}
> **Your one action this week:** {specific link}
> **Next session:** {date, topic}
> Stuck? Post in #help - someone always answers.

---

## Part 2 - The First PR Challenge (90 days)

A public, time-boxed challenge: open your first PR to a Bitcoin open-source project within 90 days. Developers don't sign up for "education pipelines" - they sign up for challenges with deadlines, prizes, and witnesses.

**Structure:**
- **Weeks 1–2:** environment + first node + pick a target repo from a curated menu (docs, tests, and good-first-issues in BDK, rust-payjoin, Floresta, peer-observer, bitcointranscripts)
- **Weeks 3–6:** attend 4+ community sessions; file a first issue or review someone's PR
- **Weeks 7–10:** build the contribution, with mentor office hours
- **Weeks 11–13:** PR opened, reviewed, iterated

**Milestones & rewards** (adapt amounts to your budget):

| Milestone | Reward |
|---|---|
| First issue filed or PR reviewed | 5,000 sats |
| PR opened | 21,000 sats |
| PR merged within 90 days | 50,000 sats + fellowship fast-track + name on the public dashboard |

**Rules that keep it honest:** upstream repos only (no PRs to your own forks) · maintainer merge = merged · AI-assisted is fine, but you walk a mentor through your diff · one entry per person.

**Public leaderboard:** a pinned message or simple page fed from your PR dashboard, updated weekly. The leaderboard *is* the marketing.

---

## Part 3 - Session formats that people talk about

### 🔴🔵 Chain Analysis Wars (2 hours)

Split the room. **Blue Team** are merchants/activists transacting on signet, trying to preserve privacy. **Red Team** plays the chain-analysis firm trying to deanonymize them with mempool.space and clustering heuristics. Then swap.

- **0:00–0:15 Briefing.** The stakes: one real story of a donation address doxxing someone. Blue mission cards: "pay 3 parties, receive from 2, consolidate once - leak nothing."
- **0:15–0:30 Setup.** Pre-funded signet wallets for Blue; Red gets a shared sheet for cluster hypotheses; facilitator holds the ground-truth ledger.
- **0:30–1:05 Round 1 - naive.** Blue uses default wallet behavior. Red hunts: address reuse, round amounts, change detection, timing. Score: +10 per correct link (Red), +10 per unlinked tx (Blue).
- **1:05–1:15 Teach break.** Name exactly which heuristics burned Blue. This is the entire privacy curriculum, taught by defeat.
- **1:15–1:50 Round 2 - armed.** Same missions with coin control, no reuse, a Payjoin between pairs, batching. The score flip is the lesson.
- **1:50–2:00 Debrief.** Map every technique to a repo: "the labeling UX that saved you → BDK issue; the Payjoin that broke clustering → rust-payjoin good-first-issues." Winners get sats. Photo. Post.

*Facilitator prep (once): 10 pre-funded signet wallets, 6 printed mission cards, ground-truth sheet. Infinitely rerunnable.*

### 🏴 Bitcoin CTF Night (6 starter challenges)

Sats locked in real (small) UTXOs that only the solver can sweep - the prize claims itself.

1. **Brainwallet graveyard** - sweep a wallet whose seed is a famous quote *(why brainwallets die)*
2. **Script kiddie** - redeem a P2SH whose script is `OP_ADD 8 OP_EQUAL` *(Script fundamentals)*
3. **Leaky change** - given 3 txids, identify payment vs change outputs *(privacy heuristics)*
4. **Nonce sense** - two signatures share a nonce; recover the key, sweep the coin *(ECDSA foot-guns)*
5. **Time lock vault** - a CLTV output that unlocks mid-session *(timelocks, guaranteed drama)*
6. **Metadata trail** - a social post + a tx + a screenshot together reveal an address *(opsec)*

Practice rounds on signet; finals on mainnet dust. Hints cost points. Publish the solutions repo afterwards - it recruits.

### 🔥 Live Fire: Merchant Deployment Day (2 hours)

Take the session to a real local merchant who's agreed to accept Bitcoin. Participants deploy the payment setup (BTCPay / a static QR solution / a Lightning wallet) *with the owner*, print the QR stand, and stay for the first real customer payment. Back at base: debrief, and **file an upstream issue for every rough edge you hit in the field** - real-world pain converted into legitimate OSS contributions. The merchant keeps every sat. This format is almost impossible for anyone to copy without a real local Bitcoin economy - if you have one, weaponize it.

### ⛏️ The Mining Race (beginner magnet)

Round 1: dice-and-whiteboard mining simulation - hash attempts are dice rolls, difficulty adjusts live, the room *feels* proof-of-work. Round 2: plug in real open-source miners (BitAxe) and lottery-mine on signet. One hour, zero prerequisites, photographs beautifully.

### 👊 Maintainer Boss Fights (monthly)

A real maintainer from a target repo reviews participants' open PRs live on a call. Participants prepare harder for this than anything else, and maintainers get cleaner PRs from your community forever after. Ask the maintainers whose repos your members already contribute to - most say yes to communities that bring them good contributors.

---

## Part 4 - Storytelling that recruits

**The dev-journey story** (one per month, thread or 60–90s video):
**Before** (who they were, honestly) → **turning point** (first session, one real struggle) → **the work** (what they built, PR links on screen) → **now** (where the code runs, what's next) → **CTA** ("They started where you are. Next session: {date}").

Rules: the subject approves before posting; tag the repo's maintainers when it goes live; link the PRs - verifiable stories beat polished ones.

**The proof-of-work habit:** every session announcement gets a follow-up comment with a screenshot of the actual call/room and what was covered. Receipts, always.

---

## Part 5 - Growth mechanics

- **Referral bounty:** bring a developer friend → you both earn sats *after their second session* (the second visit filters tourists). Cap 5 per member per cohort.
- **Guest workshops in non-Bitcoin dev communities:** your biggest untapped pool is developers who've never touched Bitcoin. Pitch GDGs, language meetups, and university CS clubs a free 90-minute **"First Commit"** session: 15 min why Bitcoin is the most interesting codebase they'll touch → 40 min hands-on (node + build a transaction) → 20 min pick a good-first-issue → 15 min the career path + community QR. Every attendee leaves with something running.
- **Partner-community slide:** one slide in allied meetups' decks - "Can you code? {Your community} turns Bitcoiners into Bitcoin builders - free." Plus a one-line forwardable message for organizers' group chats.
- **Capstone pipeline:** offer CS departments free mentorship for final-year projects that contribute to Bitcoin OSS. They get supervision; you get pre-vetted cohort members.

---

## Measuring (keep it to five numbers)

Joins → intro posts → first-session attendance → **second-session return** (the one that matters) → PRs on the dashboard. If second-session return doesn't move within two months, change the formats, not the effort.

For the reusable 60-minute developer call, one canonical weekly scorecard, and the operator rhythm for the 90-Day First PR Challenge, see [Weekly Operating Rhythm](OPERATING_RHYTHM.md).

---

*Made with 🧡 by [Code Orange Dev School](https://codeorange.dev). CC0: copy anything, ask nothing. If you run this playbook in your city, we'd love to hear about it: {contact}.*
