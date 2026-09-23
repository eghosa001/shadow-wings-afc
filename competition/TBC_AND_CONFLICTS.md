# Shadow Wings — TBC Items and Conflicts

Nothing in this file may be silently presented as settled.

## TBC — unresolved items

- exact live formation
- per-player model choices
- deployment health per agent
- current practice attempts remaining
- practice replenishment timing and carryover
- practice opponent menu/styles and repeatability
- practice cooldown
- abandon/retry/error-attempt consumption behaviour
- practice report/replay/decision-log retention
- shout duration/persistence
- shout stacking/replacement behaviour
- shout cooldown
- per-match shout limit
- exact action parameters beyond action names
- telemetry fields not yet observed
- malformed-output handling in the Virtual League
- exact agent-visible match-state details and coordinate mirroring
- same-opponent repeatability in league play
- fixture-generation timing
- deploy-failure behaviour
- wildcard weeks
- tie-break order
- prize-payment mechanics
- identity-verification deadlines
- tax/travel-document requirements
- Grand Finale T&Cs

## Conflicts — recorded, not silently reconciled

### 1. Contest Period end date

- Official Rules record transferred in the handoff: Contest Period ends November 1, 2026 12:00 UTC+8.
- Knowledge-base/registration record: final playing weekend ends October 25.
- Operating position: October 25 remains the recorded final playing date; retain the rules-period discrepancy until the current official rules are inspected directly.

### 2. Agent decision latency budget

- Transferred Virtual League KB material: roughly 5 seconds, then repeat previous action.
- Published Strands technical article: 1-second hard decision contract; a late player IDLEs for the tick.
- Operating position: live Virtual League telemetry/behaviour is the authority for Shadow Wings. Until observed, do not optimize around either timing claim.

### 3. Round numbering

- Transferred Official Rules record references "Round 8" in a prize section.
- Published season schedule in the handoff contains 7 rounds.
- Operating position: retain as a documentation conflict.

### 4. Practice quota record

- Registration email directly confirmed **up to 10 practice matches per week**.
- Older Data-Capture Protocol wording had demoted the number to unverified.
- Status: source conflict in the historical record is now **documented rather than repeated operationally**.
- Operating position: use "up to 10/week" as the registration-record ceiling, but the live portal must still provide the operational values that matter now: attempts remaining, replenishment/carryover and what consumes an attempt.

### 5. First-sample evaluation order

- Older Match-Day System material listed final score first.
- Frozen coach evaluation order places decision latency / idle-timeout rate first.
- Operating position: frozen coach order governs.

### 6. Clean-match / clean-sheet bonus value

- Current official AFC leaderboard page, checked 2026-09-23: **Clean match = +5 points**.
- Transferred KB Rev 21 material: **+10 clean sheet**.
- Status: **ACTIVE CONFLICT**.
- Operating position: do not optimize around either bonus value until current portal/rules evidence resolves it. The live leaderboard's +5 is the freshest public AFC statement currently recorded.

## Launch gate reminder

Portal-readable items above should be captured before Practice Match 1. Non-portal items remain parked unless they become decision-relevant.
