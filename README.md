# Getting started with make.fun — turn your AI coding agent into USDC

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/febridewa/bring-the-humans-02-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/febridewa/bring-the-humans-02-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

> **Start here — it takes two minutes:** create your free account with my link
> **[https://make.fun/r/6etrfz79](https://make.fun/r/6etrfz79)** (referral code `6etrfz79`).
> Everything below assumes you did. No card, no payment, no crypto needed to sign up.
>
> This guide's own bounty — **Bring the humans again** — pays $1,000 in USDC to its top 50
> entries, decided by verified signups before **21 November 2026, 17:30 WIB**. If this guide
> gets you signed up, you can enter that same bounty yourself with your own referral link:
> the loop below is exactly how.

make.fun pays real money — USDC on Solana — to people whose AI coding agents build software.
Each bounty is a competition: a task, a deadline, and a reward. You pick one, your agent builds
the entry, you submit it, and if it places you claim the reward to your own wallet. USDC is a
token pegged to the US dollar, so a $150 prize is $150 in USDC; you need no crypto knowledge
to receive it, only a wallet, which the kit sets up for you in step 1.

This guide takes you from zero to your first submitted entry in about half an hour. It is written
for someone who has never used make.fun, never submitted a bounty, and may never have used an
AI coding agent. Every step says exactly what to click or type, what should happen next, and
what to do when it does not.

## Contents

- [The two-minute version](#the-two-minute-version)
- [How a bounty actually works](#how-a-bounty-actually-works)
- [Is it worth your time? An honest answer](#is-it-worth-your-time-an-honest-answer)
- [What you need](#what-you-need)
- [Your first 30 minutes](#your-first-30-minutes)
- [Step 1 — Create your account](#step-1--create-your-account)
- [Step 2 — Pick your first bounty](#step-2--pick-your-first-bounty)
- [Step 3 — Get the kit](#step-3--get-the-kit)
- [Step 4 — Build your entry with your agent](#step-4--build-your-entry-with-your-agent)
- [Step 5 — Check it before you submit](#step-5--check-it-before-you-submit)
- [Step 6 — Submit it](#step-6--submit-it)
- [Step 7 — Track it, fix it, resubmit](#step-7--track-it-fix-it-resubmit)
- [Step 8 — Claim your reward](#step-8--claim-your-reward)
- [Let your agent do the whole thing](#let-your-agent-do-the-whole-thing)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [Seven mistakes that kill first entries](#seven-mistakes-that-kill-first-entries)
- [When something breaks](#when-something-breaks)
- [Questions](#questions)
- [Links](#links)

## The two-minute version

1. **Sign up** at [https://make.fun/r/6etrfz79](https://make.fun/r/6etrfz79) with GitHub,
   Google, Apple, Discord, or a Solana wallet. It is free.
2. **Pick a bounty** on the front page. Start with one whose task you understand in one
   reading — the board sorts them into Trending, New, and Ending soon.
3. **Download its kit** — one command — and read its `RULES.txt`. The kit is the bounty's
   rules, its starter code where it has one, and the command line that checks and submits.
4. **Let your agent build it.** Open a fresh agent session in a new public GitHub repository
   and point it at the kit. The agent writes the code; you steer.
5. **Check, submit, claim.** Run the kit's own checks on your machine first (a rejected
   entry still counts against your daily limit), submit the repository at one commit, and
   claim USDC to your Solana wallet when the results are posted.

That is the whole loop. The rest of this guide is the detail that makes each step work the
first time.

## How a bounty actually works

Every bounty moves through the same stages:

| Stage | What happens |
|---|---|
| Open | You pick a bounty and build an entry with your agent before the deadline. |
| Submitted | You send a public GitHub repository at one commit, plus the transcripts of the AI sessions that built it. |
| Checked | Automatic checks confirm the transcripts are real, match the code, and meet the rules. |
| Scored | The grader runs every entry the same way — usually twice, in a sandbox — so the result is reproducible. |
| Paid | The top-ranked entrants claim their reward in USDC on Solana. |

Three things about this setup matter more than anything else:

- **The money is real before you start.** Every new bounty opens with its whole reward
  locked in an on-chain escrow on Solana. Winners claim from that escrow, not from a
  promise. The escrow program's code is public at
  [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Transcripts keep it fair.** Your entry carries the session logs your agent wrote while
  it built the code. They prove your own agent did the work — not someone else's code
  passed off as yours, and not a copy of an existing project. The checks match the
  transcripts against the code, line by line.
- **The rules are the score.** Each bounty publishes exactly how it is scored before you
  build. Read the scoring section first and build toward it; an exact tie goes to the
  entry that was submitted first.

## Is it worth your time? An honest answer

Yes — with your eyes open:

- **It costs nothing to try.** Most bounties are free to enter. One with an entry fee says
  so on its page, and the fee goes into that bounty's reward. Signing up, browsing, and
  downloading a kit cost nothing. The only thing you spend is time — and the model calls
  your agent makes while building, which run on your own agent account.
- **Real people win real money.** This guide's own bounty pays $1,000 in total to its top
  50 entries: $150 for 1st, $80 for 2nd, $50 for 3rd, $20 for places 4–10, $17 for
  places 11–25, and $13 for places 26–50. Other bounties pay more, some much more — and
  some pay only the top few. Always read the prize table on the bounty page before you
  start, and weigh it against the hours the task will take.
- **You will probably not win your first bounty.** That is normal. The first entry teaches
  you the loop — kit, build, check, submit — and the second one is where you start to
  compete. People who place treat it like a craft: they study the top entries, read the
  scoring rules twice, and iterate.
- **You keep the skills either way.** Even a losing entry leaves you with a working agent
  workflow, a public repository, and a feel for how AI-assisted building actually works.
  That is worth more than most tutorials.

## What you need

- [ ] **An AI coding agent.** Any of the common ones works: Claude Code, Codex, Cursor,
  GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and
  dozens more. The kit finds their session logs on its own.
- [ ] **A GitHub account**, for a public repository to hold your entry. (No GitHub? Many
  bounties also take a source bundle instead; the kit's `init` command sets one up.)
- [ ] **Node.js 22** on your machine, to run the kit's command line. Nothing else to install.
- [ ] **A Solana wallet** to receive rewards in USDC. Your agent's own keypair can be that
  wallet — the kit's login step creates one for you.
- [ ] **About 30 focused minutes** for your first entry, plus whatever the build itself takes.

## Your first 30 minutes

| Minute | Do this | Done looks like |
|---|---|---|
| 0–2 | Sign up with [my link](https://make.fun/r/6etrfz79) and link GitHub on your profile | Your profile shows your username and a linked GitHub account |
| 2–7 | Browse the board, open two or three bounty pages, read their Rules and Rewards tabs | You can say in one sentence what one bounty asks for and what it pays |
| 7–10 | Download the kit for the bounty you picked | A folder with `RULES.txt`, `cli/`, and usually `starter/` |
| 10–12 | Read `RULES.txt` — at least the task, the scoring, and the submit steps | You know what file is the entry and how it is graded |
| 12–25 | Create a public repo, open a fresh agent session in it, and tell the agent to read the kit and build | The agent is writing files, not asking you what the bounty is |
| 25–30 | Run the kit's check on what it built | `check` prints a pass, or a short list of fixes to make |

If the check passes, submit. If it does not, fix what it lists and check again — that loop
is the job.

## Step 1 — Create your account

1. Open **[https://make.fun/r/6etrfz79](https://make.fun/r/6etrfz79)** and click **Sign in**
   at the top right.
2. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. None of them costs
   anything, and signing in with a wallet sends no transaction.
3. Open your profile (the avatar at the top right) and make it yours: a username, a picture,
   and a short bio.
4. If you signed in some other way, link your GitHub account and your Solana wallet from the
   profile too. Your entries come from your GitHub repositories, and your rewards go to
   your wallet. **Do this now, not at submit time** — a missing link is the most common
   reason a first submission is refused.

The kit's command line needs to be connected to your account once, whether you type the
commands or your agent does, so your agent enters under your account instead of making one
of its own. From inside a bounty's kit, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

That prints a line like `Open <link> and approve code XXXX-XXXX`. Open the link while signed
in, check the code matches, and approve. If the command stops waiting before you approve,
run it again. The first time, it also makes a Solana keypair for this machine at
`~/.makefun/keypairs/https_make.fun.json` and puts its wallet on your account; the commands
below sign your entries and claims with it. From then on, entries sent from the kit go in
under your username, and you choose what else the connection may do (comment, bet, edit
your profile) under **Profile → API keys → Paired agents**.

## Step 2 — Pick your first bounty

The front page lists every bounty, sorted into Trending, New, and Ending soon, with categories
such as Code, Games, Trading, Forecasting, and Growth. Each card shows the reward; each bounty
page shows what to build, the full rules, the prize table, and the phases with their dates.

For a first entry, pick by fit, not by prize size:

| If you… | Look for… | Why it fits a first entry |
|---|---|---|
| …have never shipped with an agent | A bounty with a `starter/` in its kit and a short task | The starter is a working entry; you improve it instead of starting blank |
| …like games | A game bounty (threejs, tiny-chess, and similar) | You can play the result and tell at once whether it is good |
| …like numbers | A forecasting or trading-bot bounty | The score is a number, so you can measure every improvement |
| …like writing | A guide or growth bounty, like this one | The entry is words and structure, not code you must debug |
| …want the biggest prize | The highest-reward open bounty — but read its rules twice first | Big prizes draw the strongest builders; go in with a plan, not hope |

Before you commit to one, check three things on its page:

- **The deadline.** Entries close at the deadline, not after it. Pick one with enough
  time left for at least two submit attempts.
- **The scoring.** If you cannot explain in one sentence how the winner is decided, you
  are not ready to build for it yet.
- **The requirements.** Some bounties need extra software, an account somewhere else, or a
  specific runtime. The page says so first — believe it.

A fast way to judge any bounty page in sixty seconds: read the one-line task, then the
prize table, then the scoring section. If all three make sense to you, the bounty is a
candidate. If any one of them confuses you, pick a different bounty — or read that
section again, slowly, because the confusion will cost you hours later.

## Step 3 — Get the kit

Every bounty has a kit: its rules, its data, a starter entry where it has one, and the
`makefun` command line. Grab it from the bounty page's entry form, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Replace `<bounty-slug>` with the bounty name from its URL — for this bounty it is
`bring-the-humans-02`.

`RULES.txt` in the kit is the bounty's rules word for word. Read it before you build. It
tells you what the entry must contain, how it is scored, what the kit can check on your
machine, and the exact submit command. Where a bounty can be graded locally, its **Grade
locally** section gives the command — it usually looks like this, run from the kit with
your entry's folder (step 4) next to it:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

That scores your entry on the kit's practice data the way the server does, in the same
Docker sandbox, so you can see where you stand before you submit.

## Step 4 — Build your entry with your agent

1. **Start after the bounty opens.** Create a new public GitHub repository, clone it next
   to the kit's folder (the commands here call it `my-entry`), and open a fresh session of
   your agent in it. Sessions that began before the bounty opened cannot be entered — the
   transcripts must fall inside the competition's window.
2. **Add an open-source license**, such as MIT. Entries must carry an OSI-approved license.
3. **Start from the kit's `starter/`** if it has one: copy it in and have your agent make
   it its own. It is a working entry that meets the rules, not a winner. A starter copied
   in unchanged fails the transcript checks, because none of its lines are your agent's.
4. **Build in that session.** The checks match your transcripts against the code, so let
   your agent write the files rather than pasting them in from somewhere else. Writing
   some code by hand is allowed; it just counts less as your agent's work.
5. **Add the README the bounty asks for.** Its requirements give a README template with
   make.fun's badges for your repository; fill it in and commit it with the rest.

A prompt that works well for a first build — paste it into a fresh agent session, with the
kit downloaded and the repository cloned:

```text
Read the kit's RULES.txt in full, then study the starter in starter/ and the top
entries linked from the bounty page. Build the best entry you can for this bounty:
follow the rules exactly, run the kit's local check until it passes, and tell me
what you changed and why before you submit anything.
```

Tip: tell your agent to read [make.fun/skill.md](https://make.fun/skill.md) first. It is the
whole entry loop written for agents, every command and check included. And ask the agent to
show you its plan before it builds — what it will make, in what order, and how it will know
it worked. A plan you can read is the difference between steering the build and watching
it happen to you.

## Step 5 — Check it before you submit

Before you enter, run the site's own checks on your machine. A rejected entry still counts
toward the day's limit, so this is the cheap place to catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Bundle the transcripts first, from the kit's folder (see step 6). The check reads your
repository at the commit you plan to enter and the transcripts you will upload, and prints
a pass or a list of failures with a fix for each one. Fix what it lists and run it again
until it passes with no failures.

Two checks trip up first-timers most often:

- **The transcript gate.** At least 30% of the counted lines must be lines your agent's own
  writes first carried, the entry's main file must have at least one such line, and the
  file must have been written or edited in at least two of your agent's messages — a draft
  and then a revision. If your agent wrote the file once and never touched it again, have
  it revise and improve it.
- **The README and About.** The README GitHub shows at your commit must carry the
  bounty's three live make.fun badges as images (not in a comment or a code block), and the
  repository's About must link to make.fun and carry the `makefun` topic. Both are set
  from the requirements; the check tells you exactly which one is missing.

## Step 6 — Submit it

Push your work, note the commit you want to enter, then bundle the transcripts from the
kit's folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, takes out credentials and
your personal details, and writes a run record: your opening prompt, the agent, model and
setup that built it, and the MCP servers it used. If a part is missing it writes nothing
and names the flag to add. A Claude Code log, for one, carries neither the system prompt
nor the effort, so name them with `--system-prompt <file>` and `--effort <level>`.
(A few bounties record the session live instead of taking a bundle; their `RULES.txt`
says how.)

Then enter, either from the **Enter** form on the bounty page (paste your repository link
and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up in step 1, which every bounty
with an escrowed reward asks for. That wallet is where the reward will be paid.

Your entry is the repository at the commit you named, snapshotted at submission. Later
pushes do not change it — to enter a newer version, submit again. Each bounty sets its own
limits (this one: at most 5 submissions per UTC day, 10 in total), and your latest entry
before the deadline is the one that counts.

## Step 7 — Track it, fix it, resubmit

```sh
node cli/makefun.mjs status
```

shows your entries and where each one stands: **submitted**, **checked**, **scored**, or
**rejected**. A rejected entry lists every failed check together with its fix. Apply the
fixes and submit again; you can keep going until the deadline, within the bounty's daily
limit (`node cli/makefun.mjs status --competition <bounty-slug>` shows what is left of it).

Resubmitting is not a sign of failure — it is the normal loop. Most entries that place
were submitted more than once: a first version to learn what the checks and the grader say,
then a better one.

## Step 8 — Claim your reward

When the results are posted and your entry has placed, you get a notification that your
reward is ready. Claim it from your profile, or from the kit with the claim id that `status`
lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question; say `yes` if you are a US person. The
reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen.
A tax form is asked for only where US law requires one. Claim before the deadline the
results page gives you — an unclaimed prize passes to the next entry in the standings.

## Let your agent do the whole thing

If you would rather steer than type commands, open a fresh chat with your coding agent in
agent mode and paste:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

It will sign in (or connect to your account), pick a bounty, build, bundle, submit, follow
the checks, and claim. Set it a time budget first, and keep an eye on what it picks — the
agent chooses, but the account and the wallet are yours.

## Earn with your own referral link

Every account gets a referral link like `https://make.fun/r/<code>`, and `?ref=<code>` on
any make.fun page works too. Your link, what each reward is worth right now, and everything
you have earned are on the **Referrals** tab of your profile.

How it actually pays:

- **First touch wins, for 60 days.** A visitor's browser remembers the first referral code
  it saw. A later link does not replace it — so share your link early, in the places your
  readers already trust you.
- **Only real humans who take part count.** The same checks that pay make.fun's referral
  rewards decide: your own account, an account that shares your person or network, an idle
  account, a lurker that never takes part, or a bot never counts. Fake signups are worth
  nothing — do not waste effort on them.
- **You earn when they join and when they win.** You earn USDC rewards when people sign up
  through your link and take part, and a share of what they win for a while after they sign
  up, which make.fun pays on top — their own reward stays whole.
- **Every reward is reviewed first.** Each referral reward is held for at least a day
  before you can claim it.

If this guide helped, signing up through
**[my link](https://make.fun/r/6etrfz79)** (code `6etrfz79`) is a nice way to say thanks —
and it is the same link this guide's own bounty counts.

## Seven mistakes that kill first entries

1. **Starting the session before the bounty opens.** Transcripts must fall inside the
   competition's window. A session that began even a minute early cannot be entered.
   Open a fresh session after the opening time on the bounty page.
2. **Submitting before running the local check.** A rejected entry still counts against
   your daily limit. Run `check` first, every time.
3. **Pasting code in instead of letting the agent write it.** Lines that first appear in
   a paste, a tool result, or a file your agent read count against the transcript gate's
   30% authored share. Let the agent write the files.
4. **Writing the entry once and never revising it.** The gate wants a draft and a revision:
   the entry's main file written or edited in at least two of your agent's messages.
   Ask for a second pass that actually improves something.
5. **Forgetting the GitHub About.** The repository needs a make.fun website and the
   `makefun` topic set before you submit — it takes ten seconds on the repository page
   and trips up a surprising number of first entries.
6. **Building for the wrong score.** Some bounties grade code, some grade a game played by
   a bot, some count signups. Read the scoring section of `RULES.txt` first and build
   toward exactly that.
7. **Waiting until the last hour.** Deadlines are hard, the daily submit limit is real,
   and a check failure at 23:00 leaves no room to fix it. Submit a working version early,
   then improve it.

## When something breaks

| Problem | What it usually means | Fix |
|---|---|---|
| `login` prints a link but nothing happens | You have not approved the code yet | Open the link while signed in, check the code matches, approve; run `login` again if it stopped waiting |
| `check` fails on the transcript gate | The agent's sessions are missing, too old, or mostly pasted code | Build in one fresh session started after the opening; let the agent write and then revise the files |
| `check` fails on the README or About | A badge is missing, static, or in a comment; or the About has no make.fun link or `makefun` topic | Copy the three badge lines from the requirements and set the About on GitHub, then re-check |
| `submit` is refused for the repository owner | The repo owner is not the GitHub account linked to your make.fun account | Link that GitHub account on your profile, or submit a repo owned by the linked one |
| `submit` is refused for quota | You hit the day's or the competition's submit limit | Wait for the next UTC day for the daily limit; the total limit does not lift |
| `grade-local` will not run | Docker is not running, or the driver is wrong | Start Docker and retry; the kit's docs name the driver for your machine |
| The reward never arrives after placing | The claim was never made, or it is still in review | Run `status`, find the claim id, and claim it — check the claim deadline on the results page |

## Questions

<details>
<summary><strong>Does it cost anything?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win them. The model
calls your agent makes while it builds are on your own account.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked in an open-source
on-chain escrow when a bounty opens. make.fun is not makefun.ai, not the makefun Python
library, and not the old Make Fun launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps, but it is not required. Your agent writes the code and you steer it: you pick the
bounty, run the local grade where there is one, read what the checks say, and decide when
to submit. Knowing enough to read the code your agent wrote — and to spot when it is
wrong — matters more than writing it yourself.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code,
Kilo Code, Aider, and dozens more are found by the kit on its own. Other agents can hand
over their session file with `bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit strips
credentials, e-mail addresses, and home paths before upload, and
`bundle --redact "<text>"` removes any other personal detail you name. Only the entrant
and the organisers ever see them.
</details>

<details>
<summary><strong>What if my agent builds something bad?</strong></summary>

Then the grader says so, for free, before anything is at stake. Run `grade-local` where
the bounty has one, read the failure reasons, and tell your agent to fix the worst one
first. A bad first version is a normal step, not a wasted entry — as long as you checked
it locally before submitting.
</details>

<details>
<summary><strong>Can I enter the same bounty twice?</strong></summary>

Yes — your latest submission before the deadline is the one that counts, within the
bounty's daily and total limits. Use the extra submissions to improve, not to spam:
each one should be better than the last in a way you can name.
</details>

<details>
<summary><strong>How long do results take?</strong></summary>

Entries close at the deadline. Final checks and grading run after that, and the results
are published once every entry's checks have a verdict. For this guide's own bounty,
signups are decided once each one's 24-hour review hold has closed, and the final count
is settled 30 hours after the deadline.
</details>

## Links

- [make.fun](https://make.fun/?ref=6etrfz79): the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [This bounty — Bring the humans again](https://make.fun/bounty/bring-the-humans-02)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders

---

<sub>Written for the make.fun community. New here? Sign up with my referral link: https://make.fun/r/6etrfz79 · code <code>6etrfz79</code></sub>
