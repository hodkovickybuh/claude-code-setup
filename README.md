<p align="center">English · <a href="README.zh-CN.md">中文</a></p>

# Claude Code setup

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/hero-c-night.svg"><img src="assets/hero-c-day.svg" alt="Pixel-art camp: Šéf with a crown at the fire, helpers at work around it." width="100%"></picture></p>

A non-coder's setup: Claude Code does the work across 8 projects. Two rules hold it together. Whoever made something doesn't judge it. Nothing is sent or published without approval.

## Request flow

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/quest-map-night.svg"><img src="assets/quest-map-day.svg" alt="Request flow in 9 steps: request, sorting, intro page (waits for answers), brief and plan, helpers work, boss loop, delivery, gate (waits for approval), save." width="100%"></picture></p>

| Step | What happens | Parts |
|---|---|---|
| 1 Request | The project opens in its own terminal profile. Rules, memory and status load. Ctrl+G can tidy the prompt first. | P02 P03 P04 P18 |
| 2 Šéf sorts it | Small: done at once. Bounded: one-line plan, up to 3 questions. Bigger: step 3. | P01 |
| 3 Intro page | A web page of questions with suggested answers ticked. **Waits for answers.** | P06 |
| 4 Brief & plan | A written brief, then steps, helpers and a cost estimate. | P01 |
| 5 Party works | Up to 3 to 4 at once, each starting from the brief. | P05 P08 P13 |
| 6 Boss loop | Independent check, see below. | P07 |
| 7 Delivery | Report split into found, estimated, proposed. "Done" only when checked. | P01 |
| 8 The gate | Anything sent, published, paid or deleted for good waits for a yes to the exact draft. **Waits for approval.** | P09 P10 P14 P15 |
| 9 Save point | Status and memory are updated for the next session. | P03 P20 P21 |

## Boss loop

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/boss-loop-night.svg"><img src="assets/boss-loop-day.svg" alt="Quality check: workers build, a fresh checker scores each criterion 0 to 10, blocking findings go back, at most 3 rounds, done at 9 or more." width="100%"></picture></p>

1. **Bar.** One concrete example of "good", never an adjective.
2. **Workers.** One helper per piece. No two touch the same file.
3. **Checker.** A new helper with no history. It opens and uses the result, then scores each criterion 0 to 10.
4. **Findings.** Blocking ones go back to the workers. Optional ones only if a round is left.
5. **End.** At most 3 rounds. Done means no blocking findings and 9 or more on every criterion.

Used for anything public and for design. Not for first drafts or small fixes.

## Safety

- A yes covers one exact draft. New content or recipients need a new yes.
- The same gate covers posting, publishing, pushing code, payments, paid generation and permanent deletion.
- One exception: status messages to my own Telegram, only when I'm away from the Mac, never 22:00 to 07:00.
- A hook blocks the worst irreversible commands even if the model forgets the rules.
- All keys live in one locked place, never in text, memory or history.
- Setup changes are versioned and backed up. Deleting means the Bin.

## Parts

| # | Part | What it is |
|---|---|---|
| P01 | Šéf | The main session's style: sorts requests, plans, delegates, reports. |
| P02 | Rules | Instructions every session reads first: a global file and 4 rule files. |
| P03 | Memory and status | Per project: memory notes for facts, a status file for what's going on. |
| P04 | Projects | 8 project folders, each with its own rules, status and terminal profile. |
| P05 | Helpers | Subagents briefed per job. Opus leads and checks, Sonnet for routine work, Haiku for lookups. |
| P06 | Intro page | Questions as a clickable page before bigger work. |
| P07 | Boss loop | The independent check above. |
| P08 | Skills | Instruction packs loaded only when needed. 35 in total, 10 start only by hand. |
| P09 | Safe stop | Nothing sent or published without a yes to the exact draft. |
| P10 | Guard hook | A script that checks commands before they run. |
| P11 | Key store | One locked place for every access key. |
| P12 | Undo trail | Version history of the setup and backups before every change. |
| P13 | Tools | MCP servers for a browser, UI components and creative apps; connectors for mail, calendar, files and docs. |
| P14 | Družina | A Mac window showing the sessions live as a pixel-art camp. Approve or deny requests from it. |
| P15 | Telegram | Requests and status on the phone when away from the Mac, with Approve and Deny buttons. |
| P16 | Stream Deck | 6 keys as a status display: sessions, usage limits, context, model, sleep. |
| P17 | Status line | Model, effort, context and usage limits at the bottom of the terminal. |
| P18 | Prompt improver | Ctrl+G rewrites a rough prompt into a clear request. |
| P19 | Event log | What each session does, as metadata only, never the content. Feeds P14, P16 and P21. |
| P20 | Save | "ulož" (save) writes status and memory at the end of work. |
| P21 | Overview | "přehled" (overview) shows every project on one screen. |

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/party-roles-night.svg"><img src="assets/party-roles-day.svg" alt="Nine helper roles and their hats: design, research, checks and security, texts, web, email, legal, finance, general." width="100%"></picture></p>

## Inventory

<p align="center"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/inventory-night.svg"><img src="assets/inventory-day.svg" alt="Inventory as of 6 October 2026: 8 projects, 35 skills (10 manual-only), 4 rule files, 206 memory notes, 22 hook registrations on 13 events, 3 MCP servers, 6 Stream Deck keys, Telegram on, 314 Družina self-checks passing, 138 helpers sent out since 4 October, 611 prompts in 7 days, 13 commits of setup history." width="100%"></picture></p>

<sub>Numbers counted by script from the setup's own files, as of 6 Oct 2026. Characters: Clawd, Anthropic's mascot, from Claude Code; the camp, hats and props were drawn for Družina. Not affiliated with Anthropic. Fonts: Pixelify Sans, IBM Plex Mono (SIL Open Font License).</sub>
