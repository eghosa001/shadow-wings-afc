# AFC Virtual League — Rules and Structure (Shadow Wings working copy)

Labels: **CURRENT PUBLIC**, **REGISTRATION RECORD**, **TRANSFERRED KB/RULES**, **PORTAL TBC**, **CONFLICT**.

## 1. Season structure

**REGISTRATION RECORD**

- September 11 to October 25, 2026.
- Friday–Sunday each week, UTC+8.
- Seven consecutive weeks.
- Round 3 recorded as Sep 25–27; later rounds continue weekly through Oct 23–25.
- Exact displayed opening/closing clock times: **PORTAL TBC**.

**CONFLICT:** transferred Official Rules record says the Contest Period ends Nov 1, 2026 12:00 UTC+8, while the playing schedule ends Oct 25.

## 2. Leagues and qualification

**REGISTRATION RECORD**

- Up to six leagues.
- Up to 2,000 teams per league.
- 10 league matches per week.
- 10 Grand Finale qualifiers: six league winners + four wildcard winners.

Transferred records additionally describe random same-league pairing, wildcard categories and best-27 ranking. These should be rechecked against current rules before being used for optimization.

## 3. Scoring

**CURRENT PUBLIC**

- Current AFC leaderboard says **Clean match = +5 points**.

**TRANSFERRED KB Rev 21**

- Win +30, Draw +10, Loss +2.
- +6 per goal margin, max +30.
- +10 clean sheet.
- +8 per win from the third consecutive win.

**CONFLICT:** +5 current leaderboard vs +10 transferred KB for a no-concession match.

**Operating rule:** do not optimize around the disputed clean-match value until current portal/rules evidence resolves it.

## 4. Practice matches

**REGISTRATION RECORD**

- Up to 10 practice matches per week.
- Practice matches award no points.

**PORTAL TBC**

- current remaining attempts
- replenishment/carryover
- opponent menu and repeatability
- cooldown
- retry/abandon/error attempt consumption
- report/replay/log retention

## 5. Competitive matches

**REGISTRATION RECORD**

- 10 league matches per week.
- Find opponent can initiate a match; matches can also auto-play.
- Prompt/model changes require **Redeploy changes**.

Transferred KB material records 2-minute automated matches, a 30-minute real-match cooldown and prompt locking while a match runs. Recheck live behaviour before relying on cooldown details.

## 6. Match engine

**CURRENT TECHNICAL SOURCE — Strands article**

- 5v5.
- Decision point about every 2 seconds in the described implementation.
- Structured actions include MOVE_TO, PASS, SHOOT, DRIBBLE, PRESS_BALL, MARK, INTERCEPT, TACKLE, CLEAR, IDLE, plus goalkeeper-specific actions.
- Described implementation uses a 1-second hard response contract and IDLE on timeout.

**CONFLICT:** transferred Virtual League KB material records roughly 5 seconds / repeat previous action.

**Operating rule:** Shadow Wings live telemetry is the authority for Virtual League timing.

## 7. Coach shouts

**CURRENT PUBLIC — official tutorial**

- Up to 200 characters.
- Sent to every agent on the pitch.
- Match clock keeps running.

Transferred tactical interpretation treats shouts as advisory context; the Strands article likewise describes free-text human guidance as context agents may or may not follow.

**PORTAL TBC:** persistence, stacking, cooldown, per-match limit, report timestamps.

## 8. Match reports and telemetry

Transferred records say reports are generated after fixtures and expose score/timeline plus agent-level analytics. Exact current fields and retention remain **PORTAL TBC**.

## 9. Fair play

Transferred rules/KB records prohibit multiple accounts, bots/scripts/automation/emulators touching the competition, collusion/result manipulation, impersonation and scraping/republishing competition data.

Shadow Wings project automation is therefore restricted to off-platform documentation, analysis and version control.

## 10. Prizes and Grand Finale

**REGISTRATION RECORD**

- Grand Finale at AWS re:Invent, Las Vegas.
- 10 Virtual League qualifiers.
- USD 50,000 prize pool.
- USD 30,000 / 15,000 / 5,000 top-three prizes.

Other travel, notification and eligibility details remain in the transferred rules record and should be rechecked when decision-relevant.
