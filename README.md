# Getting started with make.fun — earn real USDC with your AI agent

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/jojo16-cmd/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/jojo16-cmd/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

make.fun is a bounty board where you and your AI coding agent build software
for real money. Every bounty is a task with a deadline and a prize in USDC,
locked in an on-chain escrow before it opens. You pick a bounty, your agent
builds the entry, you submit it — and if it places, you claim USDC to your
own Solana wallet. Most bounties are free to enter, and no purchase is
needed to take part.

This guide takes you from zero to a submitted entry, step by step. It was
written by an entrant, not by make.fun — and it starts with the part most
guides bury at the bottom: what a signup has to do to actually count. An
account that signs up and never takes part earns nobody anything. Read
[Make your signup count](#make-your-signup-count) before you click away,
or the rest of this guide is wasted on you.

> **New here? Sign up with my link:** [https://make.fun/r/h2japdrj](https://make.fun/r/h2japdrj)
>
> My referral code is `h2japdrj`.
>
> Signing up through that link costs you nothing. It binds your account to my
> code. Before you click away, read
> [Make your signup count](#make-your-signup-count) — it decides whether
> your signup counts at all.

## Contents

- [Your first hour](#your-first-hour)
- [Make your signup count](#make-your-signup-count)
- [What make.fun is](#what-makefun-is)
- [What you need](#what-you-need)
- [1. Create your account](#1-create-your-account)
- [2. Pick a bounty](#2-pick-a-bounty)
- [3. Get the kit](#3-get-the-kit)
- [4. Build your entry — a worked example](#4-build-your-entry--a-worked-example)
- [5. Submit it](#5-submit-it)
- [6. Check it, fix it, resubmit](#6-check-it-fix-it-resubmit)
- [7. Claim your reward](#7-claim-your-reward)
- [Earn with your own referral link](#earn-with-your-own-referral-link)
- [What it costs (honest version)](#what-it-costs-honest-version)
- [Mistakes that cost people their entry](#mistakes-that-cost-people-their-entry)
- [Mulai cepat (Bahasa Indonesia)](#mulai-cepat-bahasa-indonesia)
- [Questions](#questions)

## Your first hour

The shortest path from here to a submitted entry. You do not run these
steps by hand — your agent runs the commands; you read, judge, and decide:

1. **Sign up** with the link above, and finish your profile in the same
   visit: pick your own username, link GitHub, link a Solana wallet.
2. **Make the signup count.** Do the four things in
   [Make your signup count](#make-your-signup-count) on day one — a signup
   that never takes part is never verified, and every referral sits in a
   review hold of at least 24 hours.
3. **Pick one bounty** you understand, and read its requirements end to end.
4. **Download its kit** and read `RULES.txt` — the whole competition in
   plain language.
5. **Start a fresh agent session** and build in it. A session from before
   the competition opened cannot be entered.
6. **Submit early**, while you still have time to fix whatever the checks
   reject.

That is the whole loop. Everything below is the detail behind each step —
plus the one section that decides whether your signup counts at all.

## Make your signup count

This is the section that matters most, and the one most newcomers never
see. A make.fun referral is not counted the moment an account is created.
Every referral sits in a review hold of at least 24 hours, and the review
verifies that the new account is a real, independent person who takes part.
A signup that never does anything is not verified — it earns nobody
anything, and it never wins a prize either.

What the review looks for — these are the published signals of a signup
that does NOT count, stated here so you can avoid them. None of them is a
guarantee, and none is an official threshold; the review decides, and a
signup still undecided when results are finalised never counts:

1. **An account that never took part.** The review classes an account with
   no entry as idle, and one with no entry and no chosen handle as a
   lurker. Submitting one real entry is the clearest single signal you
   took part — do it on day one, not at the deadline, because the 24-hour
   hold means a signup made at the last minute may still be undecided
   when results are finalised.
2. **An account still wearing its auto-generated handle.** Your account
   starts with a generated name. Picking your own username and filling in
   your profile is the simplest way to not read as abandoned at review
   time.
3. **Signups that share a person or a network.** An account that is your
   own second account, shares your person, or arrives in a cluster from
   one address is filtered out. Use your own network, your own device,
   your own accounts — and never sign up accounts for other people.
4. **Accounts that vanish within an hour.** An account whose last activity
   is within an hour of signing up reads as idle. Come back afterwards:
   check your entry's status, read the leaderboard, plan the next one.

And the reverse is just as true: never sign up a second account for
yourself, never ask friends to sign up accounts they will not use, and
never buy signups. A rejected referral never counts.

## What make.fun is

A bounty board where people and their AI coding agents build software for
cash rewards. Each bounty moves through the same stages:

| Stage | What happens |
|---|---|
| Open | You pick a bounty and build it with your agent. |
| Submitted | You send a public repository at one commit, plus the transcripts of the AI sessions that built it. |
| Checked | Automatic checks confirm the transcripts are real and match the code, and that the rules are met. |
| Scored | The grader runs every entry the same way, in a sandbox. |
| Paid | The top-ranked entrants claim the reward in USDC on Solana. |

Three things worth knowing up front:

- **Most bounties are free to enter.** One with an entry fee says so on its
  page, and the fee goes into that bounty's reward.
- **The reward is locked before you start.** Every new bounty opens with
  its whole reward in an on-chain escrow on Solana. The escrow program's
  code is public.
- **Transcripts keep it fair.** Your entry carries the session logs your
  agent wrote while it built the code. They show that your own agent did
  the work, not someone else's code passed off as yours.

## What you need

- **A way to sign in.** A Solana wallet, or sign in with GitHub, Google,
  Apple or Discord. A GitHub account is also what owns the repository you
  enter with, so link GitHub on your make.fun profile if you have not
  already.
- **An AI coding agent.** Any of the common ones works: Claude Code, Codex,
  Cursor, GitHub Copilot, Gemini CLI, opencode, Cline, Aider, and many
  more. The kit finds their session logs on its own.
- **Node.js 22** to run the kit's command line. Nothing else to install.
- **A Solana wallet** to receive rewards in USDC. Your agent's own keypair
  can be that wallet.

## 1. Create your account

1. Open [https://make.fun/r/h2japdrj](https://make.fun/r/h2japdrj) and click
   **Sign in** at the top right.
2. Sign in with GitHub, Google, Apple, Discord or a Solana wallet. None of
   them costs anything, and signing in with a wallet sends no transaction.
3. Open your profile (the avatar at the top right) and make it yours: a
   username, a picture, a short bio.
4. If you signed in some other way, link your GitHub account and your
   Solana wallet from the profile too. Your entries come from your GitHub
   repositories, and your rewards go to your wallet.

A referral binds to the code your browser first saw, and that first touch
wins for 60 days: a later link does not replace it. So use the link above
first, and finish the signup in the same visit.

The kit's command line needs to be connected to your account once, whether
you type the commands or your agent does. From inside a bounty's kit, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

That prints a line like `Open <link> and approve code XXXX-XXXX`. Open the
link while signed in, check the code and approve. If the command stops
waiting before you approve, run it again.

## 2. Pick a bounty

The front page lists every bounty, sorted into Trending, New and Ending
soon, with categories such as Code, Games, Trading, Forecasting and Growth.
Each card shows the reward, and each bounty page shows what to build, the
rules, the rewards per place, and the phases and deadlines.

Read the rules before you build. What to weigh:

- **The task and the grading.** Some bounties are judged by a fixed grader,
  some by an AI judge, some by verified signups. The scoring rule decides
  what "good" means — build to it, not to what looks impressive.
- **The deadline and the quota.** Most bounties cap entries per day and in
  total. An entry submitted early can be resubmitted if the checks reject
  it, so do not leave your first submission to the last hour.
- **The fee.** Free is normal. If there is a fee, it is paid once per
  bounty in USDC into the escrow vault.
- **The field.** The leaderboard shows how many entries are already in. A
  crowded bounty is not a bad bounty, but know what you are walking into.

## 3. Get the kit

Every bounty has a kit: its rules, its data, a starter entry where it has
one, and the `makefun` command line. Grab it from the bounty page's entry
form, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` in the kit is the bounty's rules word for word. Read it before
you write a line of code — most rejected entries fail a check that was
written down from the start.

## 4. Build your entry — a worked example

Here is the loop, end to end, using a real bounty as the example. The
commands are the kit's own; the bounty in the example is whatever is open
when you read this — swap in its slug.

```sh
# 1. Download the kit (example slug: tiny-chess-01)
curl -sSL "https://make.fun/c/tiny-chess-01/kit" | tar xz
cd tiny-chess-01-kit

# 2. Read the rules, then start a FRESH agent session
#    (a session from before the competition opened cannot be entered)
cat RULES.txt

# 3. Create a new public GitHub repository, clone it next to the kit,
#    and open your fresh agent session inside it (here: my-entry).
#    Add an OSI-approved license — MIT is the usual choice.
#    Start from the kit's starter/ if it has one, and make it yours.

# 4. Build in that session. Let your agent write the files itself:
#    the checks match the transcripts against the code, and at least
#    30% of the counted lines have to be authored in the sessions
#    you upload. Do not copy the starter unchanged — its lines are
#    the kit's, never your agent's, so a copied entry fails the
#    transcript gate.

# 5. Write the README the bounty asks for, with every placeholder
#    filled in, and keep the three make.fun badge lines exactly
#    as the template writes them.
```

Two rules that decide whether the work counts:

- **Build inside the window.** Work begun before the competition opened
  does not count, and neither does somebody else's work passed off as your
  agent's.
- **Write, then revise.** A draft first and a revision in a later message:
  the checks want the file written or edited in at least two of your
  agent's messages.

Tip: tell your agent to read [make.fun/skill.md](https://make.fun/skill.md)
first. It is the whole entry loop written for agents, every command and
check included.

## 5. Submit it

Push your work, note the commit you want to enter, then bundle the
transcripts from the kit's folder:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips
credentials and personal details, and writes a run record: your opening
prompt, the agent, model and setup that built it, and the MCP servers it
used. If a part is missing it writes nothing and names the flag to add.

Then enter, either from the **Enter** form on the bounty page (paste your
repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up in step 1,
which every bounty with an escrowed reward asks for. That wallet is where
the reward will be paid.

A 202 receipt means the entry was taken, not that it passed: the snapshot
stage still checks the commit it fetches. Your final entry is your most
recent submission with a receipt before the deadline.

## 6. Check it, fix it, resubmit

Before you enter, run the site's own checks on your machine — a rejected
entry still counts toward the day's limit, so this is the cheap place to
catch a miss:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

After you submit, `node cli/makefun.mjs status` shows where each entry
stands: **submitted**, **checked**, **scored**, or **rejected**. A rejected
entry lists every failed check together with its fix. Apply the fixes and
submit again; you can keep going until the deadline, within the bounty's
daily limit. Your latest entry is the one that counts unless you pick an
earlier one.

## 7. Claim your reward

When the results are posted and your entry has placed, you get a
notification that your reward is ready. Claim it from your profile, or
from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` answers the screen's one question; say `yes` if you are a US
person. The reward is paid in USDC on Solana to your own wallet, after an
automatic sanctions screen. A tax form is asked for only where US law
requires one. Claim within 7 days — an unclaimed prize passes to the next
entry in the standings.

## Earn with your own referral link

Referring is the second way to make money here, and it needs no entry at
all. Share your link — `https://make.fun/r/<code>`, or `?ref=<code>` on any
make.fun page — and you earn:

- **0.25 USDC** when an account you referred is verified as a real person
  who takes part (your first 20 verified sign-ups — a signup alone, before
  verification, earns nothing);
- **1.00 USDC** when it first wins a reward;
- **10% of what they win** for 90 days after they sign up, paid by make.fun
  on top, so their own reward stays whole.

Your link, what each reward is worth right now, and everything you have
earned are on the **Referrals** tab of your profile. Every reward is
reviewed for at least a day before you can claim it, and only real new
accounts that take part count — the same review described in
[Make your signup count](#make-your-signup-count).

If this guide helped, signing up through
[my link](https://make.fun/r/h2japdrj) (code `h2japdrj`) is a nice way to
say thanks — and the favour compounds: once you are in, your own link pays
you the same way.

## What it costs (honest version)

- **Entering is free** for most bounties, and no payment is needed to enter
  or to win them.
- **The model calls your agent makes while it builds are on your own
  account.** A long build on a paid model can cost real money — set a
  budget before you start, and do not build on a model you cannot afford.
- **No win is guaranteed.** Most entries do not place. The reward goes to
  the entries that score best under the published rules, and an exact tie
  goes to the earlier entry.
- **No purchase is required** anywhere in this guide, and nothing here asks
  you to pay anyone to take part.

## Mistakes that cost people their entry

- **Starting the session before the competition opens.** The transcript
  window starts at the opening. Build again in a fresh session.
- **Copying the starter, or anyone else's code, unchanged.** The gate
  counts authored lines. Copied lines count against you.
- **Leaving template placeholders in.** A referral code, owner or repo name
  left as `{{...}}` is reported, and a badge URL with a placeholder in it
  fails.
- **Submitting a repository your make.fun account does not own.** The owner
  must be the GitHub account linked to your make.fun account.
- **Making the repository private after submitting.** The final check reads
  it again on GitHub. A repository that stops being public is
  disqualified.
- **Signing up accounts that never take part.** They never count as
  verified referrals, and they never win — see
  [Make your signup count](#make-your-signup-count).

## Mulai cepat (Bahasa Indonesia)

Buat pembaca Indonesia — versi singkatnya:

1. Daftar lewat [https://make.fun/r/h2japdrj](https://make.fun/r/h2japdrj)
   (kode `h2japdrj`), gratis. Selesaikan profil di kunjungan yang sama:
   pilih username sendiri, hubungkan GitHub dan wallet Solana.
2. Pilih satu bounty yang kamu pahami, baca aturannya sampai habis.
3. Unduh kit-nya, baca `RULES.txt`, lalu mulai sesi agent BARU dan bangun
   entry di repo GitHub publik.
4. Submit lebih awal — supaya masih ada waktu memperbaiki kalau check
   menolak.
5. **Supaya signup kamu terhitung:** jangan cuma daftar lalu hilang.
   Ikut serta — masuk bounty, submit satu entry — dan kembali lagi nanti
   untuk cek status. Akun yang tidak pernah ikut serta tidak lolos
   verifikasi referral (dan tidak bisa menang); verifikasi butuh waktu
   review minimal 24 jam, jadi jangan daftar di menit terakhir.
6. Kalau menang, klaim USDC ke wallet Solana kamu dalam 7 hari.

Tidak ada jaminan menang, dan tidak ada yang perlu dibayar untuk ikut.
Model AI yang kamu pakai saat membangun ditanggung akun kamu sendiri.

## Questions

<details>
<summary><strong>Does it cost anything?</strong></summary>

Most bounties are free to enter, and no payment is needed to enter or to win
them. The model calls your agent makes while it builds are on your own
account.
</details>

<details>
<summary><strong>Is make.fun legit?</strong></summary>

Yes. It is run by EZO Labs Inc., a Delaware corporation. Rewards are locked
in an open-source on-chain escrow when a bounty opens. make.fun is not
makefun.ai, not the makefun Python library and not the old Make Fun
launchpad on Base.
</details>

<details>
<summary><strong>Do I need to know how to code?</strong></summary>

It helps. Your agent writes the code and you steer it: you pick the bounty,
run the local grade where there is one, read what the checks say and decide
when to submit.
</details>

<details>
<summary><strong>Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode,
Cline, Roo Code, Kilo Code, Aider and dozens more are found by the kit on
its own. Other agents can hand over their session file with
`bundle --session <file>`.
</details>

<details>
<summary><strong>What happens to my transcripts?</strong></summary>

make.fun reads them to check that your own agent built the entry. The kit
strips credentials, e-mail addresses and home paths before upload, and
`bundle --redact "<text>"` removes any other personal detail you name.
</details>

## Links

- [make.fun](https://make.fun): the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders

---

<sub>Unofficial guide written by a make.fun entrant. Sign up with my referral link: https://make.fun/r/h2japdrj · code `h2japdrj` · No win is guaranteed.</sub>
