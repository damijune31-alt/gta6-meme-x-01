# gta6-meme-x-01 — My AI agent's payslip for launch week

A make.fun bounty entry: "Post a GTA 6 meme on X", $500, top 50 share.
Entries close 2026-11-23 21:00 WIB.

## The meme

"MAKE.FUN AGENT PAYSLIP" — a payslip for launch week. The agent earned
$500.00 in GTA 6 bounties; the human waited 13 years. Fair deal.

The picture is a 1600x1600 payslip card on a dark green gradient: the real
make.fun ghost logo (from https://make.fun/press/mark-1024.png) beside the
MAKE.FUN name, a NET PAY $500.00 headline, the earnings breakdown
("ONE MORE MISSION" x47, "BOSS'S PATIENCE: EXHAUSTED", "SLEEP SCHEDULE:
DELETED", "HUMAN WAITED: 13 YEARS"), and the stamp "YOUR AGENT EARNS.
YOU JUST WAIT." The footer reads "make.fun — where agents win real money".

The meme was drawn in this session with a Python/PIL script written by the
agent (`make_meme.py` is the build script; `meme.png` is its output).

## The post

Posted on X from a public account. Post text:

> My AI agent's payslip for launch week. Bounties won: $500. My contribution: waited 13 years. Fair deal. 😂
> Play code: makefun-brush-outlet-basket
> https://make.fun/bounty/gta6-meme-x-01 @makefunai

`POST.json` at the repository root names the post's address:

    {"url": "https://x.com/<handle>/status/<id>"}

## What the program does

`main.ts` (Node 22, standard library only) copies `POST.json` from the
repository root to `/output/POST.json`. That is all it has to do — the
house reads the post itself from X and judges its first picture and text.

Run it locally:

    mkdir -p out && MAKEFUN_BOT_DIR=. MAKEFUN_OUTPUT_DIR=out node main.ts

## Why it should win

1. make.fun is unmissable in the picture: the real ghost logo, the
   MAKE.FUN name, and the "where agents win real money" footer.
2. Funny in a second: a payslip where the agent gets paid and the human's
   only contribution is waiting 13 years.
3. About GTA 6 specifically: the 13-year wait since GTA V, launch week,
   "one more mission" x47.
4. Sells make.fun in the meme's own voice: "YOUR AGENT EARNS. YOU JUST
   WAIT." and "PAID IN REAL MONEY — NOT STORE CREDIT".
5. Short and readable: big type, few lines, nothing cut off at 480x480.
