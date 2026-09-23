# Shadow Wings — Confirmed Facts

This file separates current public-source facts, direct registration-record facts and internal project facts. Conflicts are not hidden; see `TBC_AND_CONFLICTS.md`.

## Current public AFC sources — checked 2026-09-23

- The current AFC leaderboard defines a **Clean match** as a match finished without conceding and says it is worth **+5 points**.
  - Source: https://agenticfootballcup.ai/leaderboard
- The official in-game tutorial says a coach shout can contain **up to 200 characters** and goes to **every agent on the pitch** while play continues.
  - Source: https://agenticfootballcup.ai/tutorial?step=in-game
- The official team tutorial shows five agent slots and identifies the portal's default formation as **2-1-1**, while also showing formation can be changed.
  - Source: https://agenticfootballcup.ai/tutorial?step=team
  - Shadow Wings' actual live formation remains TBC; never infer it from the tutorial default.
- Published Strands technical material describes 5v5 play, a decision point about every 2 seconds, a 1-second hard response contract in that implementation, and the structured action vocabulary including MOVE_TO, PASS, SHOOT, DRIBBLE, PRESS_BALL, MARK, INTERCEPT, TACKLE, CLEAR and IDLE.
  - Source: https://strandsagents.com/blog/inside-agentic-football-cup/
  - This timing claim conflicts with transferred Virtual League KB timing; see TBC file.

## Direct registration-record facts

- AFC Virtual League runs September 11 to October 25, Friday–Sunday, UTC+8, for seven consecutive weeks.
- Up to six leagues, up to 2,000 teams each.
- Up to 10 practice matches per week.
- Practice matches award no points.
- 10 league matches per week.
- League matches can be initiated with **Find opponent** or allowed to auto-play.
- Prompt/model changes require **Redeploy changes**.
- 10 Grand Finale qualifiers: six league winners + four wildcards.
- Grand Finale is at AWS re:Invent in Las Vegas.
- Prize pool: USD 50,000; USD 30,000 / 15,000 / 5,000 for top three.

## Internal Shadow Wings facts

- Team: Shadow Wings.
- League: C.
- Prompt Set V2 frozen 2026-09-23.
- Shout Playbook V1.1 frozen 2026-09-23.
- Capture Protocol v1.1 ready.
- Practice matches played: 0 at handoff.
- League matches played: 0 at handoff.
- Formation, player models and deployment health require a live portal read.

## Source-specific transferred claims

Transferred KB Rev 21 material recorded:

- Win +30, Draw +10, Loss +2.
- +6 per goal margin up to +30.
- +10 clean sheet.
- +8 per win from the third consecutive win.

Because the current public leaderboard says Clean match +5, the clean-match component is **not treated as settled**. See `TBC_AND_CONFLICTS.md`.

## Not stored

Registration email address, passwords, keys, tokens, cookies, private portal URLs and billing information are not stored here.
